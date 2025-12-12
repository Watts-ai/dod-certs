# DoD Certificate Bundle

Automated, up-to-date bundle of Department of Defense (DoD) PKI certificates.

Certificates are updated nightly. Docker images will require rebuilds if certificates go out of date.

**Note:** APT and RPM repositories are currently in development for easier package management.

## Download

**https://go.watts.ai/dod-certs**

## Installation

```bash
curl -fsSL https://go.watts.ai/dod-certs | install -D /dev/stdin /usr/local/share/ca-certificates/dod-certificates.crt
update-ca-certificates
```

## License

See [LICENSE](LICENSE) for details.
