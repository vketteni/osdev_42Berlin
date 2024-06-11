
**RUN QEMU AARCH64
```
qemu-system-aarch64 -cpu cortex-a57 -M virt -nographic \
-drive if=pflash,format=raw,readonly=on,file=AAVMF_CODE.fd \
-drive if=pflash,format=raw,file=AAVMF_VARS.fd \
-drive format=raw,file=fat:rw:esp
```
