# Copyright (c) 2016-2024 Crave.io Inc. All rights reserved
FROM accupara/golang:1.22-bullseye

RUN set -x \
 && cd /tmp \
 && git clone https://github.com/kubernetes-sigs/vsphere-csi-driver.git vsphere-csi-driver \
 && cd vsphere-csi-driver \
 && make build \
# Cleanup
 && cd .. ; rm -rf vsphere-csi-driver
