<h1 align="center">regfish</h1>

<p align="center"><strong>API-first automation for domains, DNS, and TLS.</strong></p>
<p align="center">From DNS record changes to certificate issuance and unattended renewals.</p>

<p align="center">
  <a href="https://regfish.com/docs">Developer Hub</a> |
  <a href="https://regfish.com/docs/dns">DNS API</a> |
  <a href="https://regfish.com/docs/tls">TLS API</a> |
  <a href="https://regfish.com/docs/recipes">Recipes</a>
</p>

regfish has been building domain, DNS, and TLS infrastructure since 2002. On GitHub we publish the open-source building blocks around our APIs: clients, integrations, and utilities that turn DNS changes and certificate workflows into something you can actually automate.

<table>
  <tr>
    <td valign="top" width="50%">
      <strong><a href="https://regfish.com/docs">Developer Hub</a></strong><br />
      The central entry point for the regfish API platform, including authentication, API references, schemas, and next steps.
    </td>
    <td valign="top" width="50%">
      <strong><a href="https://regfish.com/docs/recipes">Recipes</a></strong><br />
      Step-by-step workflows for common DNS and TLS tasks, from safe DNS updates to explicit renewal and reissue cycles.
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong><a href="https://regfish.com/docs/dns">DNS API</a></strong><br />
      Read, create, update, and delete DNS records for automated zone and validation management.
    </td>
    <td valign="top" width="50%">
      <strong><a href="https://regfish.com/docs/tls">TLS API</a></strong><br />
      Order, manage, revoke, and download TLS certificates programmatically.
    </td>
  </tr>
</table>

## Open source that ships with the platform

- [certbro](https://github.com/regfish/certbro) is our open-source Linux CLI built on top of the regfish DNS API and TLS API. It provisions `dns-cname-token` validation records, downloads issued certificates, rotates keys, deploys stable PEM paths, and keeps unattended renewals manageable on real servers.
- [regfish-dnsapi-go](https://github.com/regfish/regfish-dnsapi-go) is the official Go client for the regfish DNS API.
- [libdns/regfish](https://github.com/libdns/regfish) brings regfish DNS into the `libdns` ecosystem.
- [caddy-dns/regfish](https://github.com/caddy-dns/regfish) adds regfish as a DNS provider for Caddy's ACME DNS challenge flow.
- We also maintain integrations for tools such as [lego](https://github.com/go-acme/lego) and [Lexicon](https://github.com/AnalogJ/lexicon), so regfish fits into existing DNS and TLS stacks.

## Good starting points

- Want end-to-end Linux certificate automation? Start with [certbro](https://github.com/regfish/certbro) and the recipe [TLS automation with DNS API](https://regfish.com/docs/recipes/tls-automation-regfish-dns-api).
- Need safer record changes? Pair the [DNS API](https://regfish.com/docs/dns) with [DNS record update with rollback](https://regfish.com/docs/recipes/dns-record-update-with-rollback).
- Optimizing certificate lifecycles? See [Maximize TLS lifetime with reissue cycle](https://regfish.com/docs/recipes/maximize-tls-lifetime-with-reissue-cycle) and [TLS explicit renewal](https://regfish.com/docs/recipes/tls-explicit-renewal).

## Build with regfish

If you want the raw building blocks, start in the [Developer Hub](https://regfish.com/docs). If you want copyable workflows, go straight to [Recipes](https://regfish.com/docs/recipes). If you want a ready-to-run server tool, use [certbro](https://github.com/regfish/certbro).
