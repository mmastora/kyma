FROM eu.gcr.io/kyma-project/incubator/develop/k8s-tools:20210113-12c4e3b5

RUN apk add --no-cache jq apache2-utils

COPY ./scripts/config_replace.sh /

LABEL source=git@github.com:kyma-project/kyma.git

ENTRYPOINT ["/bin/bash", "/config_replace.sh"]
