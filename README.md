# data-services-nest

A [nuthatch](https://github.com/nightswatchhq/nuthatch) nest of provider registrations on Arbitrum One
for five community Horizon data services: Dispatch, Seahorn, SDSCE, Mainline and the Nuthatch Data
Service. It holds `ProviderRegistered(address,string,string)` and `ProviderDeregistered(address)` and
nothing else, one pair of tables per service (`dispatch__provider_registered`, ...).

Lodestar's service census reads it through kittiwake.

```sh
nuthatch dev --window 25000
```
