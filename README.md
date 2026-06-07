
```
Want to get into the world of DevSecOps? In this video we go over important DevSecOps Principles like SCA, SAST, SBOM, SecretScanners and removing vulnerabilities by reducing your security footprint with Distroless images.
 
Distroless Images article: https://edu.chainguard.dev/chainguard/chainguard-images/about/getting-started-distroless/

Chainguard NGINX Image: https://images.chainguard.dev/directory/image/nginx/overview?utm_source=bradmorgan&utm_medium=devinfluencers&utm_campaign=FY25-DevInfluencers

Eraser Whiteboard: https://app.eraser.io/workspace/lV8r8PWZCwuASvuEf5wF

Docker Desktop: https://www.docker.com/products/docker-desktop/

Repo with Code: https://github.com/rapXidy/DevSecOps-nginx


docker scout cves $APP_NAME:$VERSION --output ./vulns.report
docker scout cves $APP_NAME:$VERSION --only-severity critical --exit-code
docker scout sbom --output $APP_NAME.sbom $APP_NAME:$VERSION


#TEST: Run the container
docker run -d -p 80:80 --name $APP_NAME webapp
```