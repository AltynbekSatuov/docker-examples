# escape=`

ARG BASE_IMAGE
ARG SPE_IMAGE
ARG HEADLESS_SERVICES_IMAGE

FROM ${SPE_IMAGE} as spe
FROM ${HEADLESS_SERVICES_IMAGE} as headless_services
FROM ${BASE_IMAGE}

COPY --from=spe C:\module\db C:\resources\spe
COPY --from=headless_services C:\module\db C:\resources\jss