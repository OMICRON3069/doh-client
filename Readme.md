DNS-over-HTTPS Client
==============

Client software to query DNS over HTTPS, using [Google DNS-over-HTTPS protocol](https://developers.google.com/speed/public-dns/docs/dns-over-https)
and [IETF DNS-over-HTTPS (RFC 8484)](https://www.rfc-editor.org/rfc/rfc8484.txt).

Note: This is a fork from origional project to meet my personal need, i.e. to provide a DoH client without UDP DNS, and it's still under construction.(You may use original project for general purpose)

## Redesigned Upstream Schema

Inspired by [PersonalDNSFilter](https://github.com/IngoZenz/personaldnsfilter), I choose to set upstreams by IP, not domain.

For example:
```
8.8.8.8::443::IETF::https://dns.google/dns-query

[2001:4860:4860::8888]::443::IETF::https://dns.google/dns-query
```

## Other Considerations

- Change from toml to yaml
- Ability to set custom UA

## License

DNS-over-HTTPS is licensed under the [MIT License](LICENSE). You are encouraged
to embed DNS-over-HTTPS into your other projects, as long as the license
permits.

You are also encouraged to disclose your improvements to the public, so that
others may benefit from your modification, in the same way you receive benefits
from this project.
