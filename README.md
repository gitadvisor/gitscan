Github Scan Github Action

Scan an image uploaded to ECR and fail if vulnerabilities are found.
Quick Start

      - name: Scan Docker image
        id: docker-scan
        uses: cvedb/gitscan@v1.0
        with:
          repository: myorg/myimage
          tag: v1.2.3
          fail_threshold: high
