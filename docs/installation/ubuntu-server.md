# Foundation installation plan

Status: In progress; installation media not yet confirmed.

1. Back up infrastructure node data and prepare Windows recovery media if needed.
2. Download Ubuntu Server 24.04 LTS AMD64 from https://ubuntu.com/download/server.
3. Use balenaEtcher (Intel macOS version) on the management node to flash a USB drive. Verify the selected target; flashing erases it.
4. Validate the USB and safely eject it.
5. Boot the infrastructure node from USB and verify the intended installation disk before erasing Windows.
6. Install Ubuntu Server with hostname `infra-01` and OpenSSH.
7. Verify OS, hardware, networking and SSH; configure updates and secure remote access.
8. Test power, lid behavior and cooling before enabling continuous operation.

Record actual commands, outcomes and troubleshooting here as implementation progresses.

References: https://ubuntu.com/server/docs and https://etcher.balena.io/.
