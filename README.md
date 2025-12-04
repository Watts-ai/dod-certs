# DoD Certificate Bundle

Automated, up-to-date bundle of Department of Defense (DoD) PKI certificates.

Certificates are updated nightly. Docker images will require rebuilds if certificates go out of date.

**Note:** APT and RPM repositories are currently in development for easier package management.

## Download

**https://go.watts.ai/dod-certs**

## Installation

### Ubuntu/Debian

```bash
curl -o /usr/local/share/ca-certificates/dod-certificates.crt https://go.watts.ai/dod-certs
update-ca-certificates
```

### Alpine

```bash
curl -o /usr/local/share/ca-certificates/dod-certificates.crt https://go.watts.ai/dod-certs
update-ca-certificates
```

### Docker

**Ubuntu/Debian:**
```dockerfile
RUN curl -o /usr/local/share/ca-certificates/dod-certificates.crt https://go.watts.ai/dod-certs && \
    update-ca-certificates
```

**Alpine:**
```dockerfile
RUN curl -o /usr/local/share/ca-certificates/dod-certificates.crt https://go.watts.ai/dod-certs && \
    update-ca-certificates
```

## License

See [LICENSE](LICENSE) for details.
