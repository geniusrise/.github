![logo_with_text](https://github.com/geniusrise/.github/assets/144122/2f8e51ee-0fcd-4f74-90fd-97301ef7943d)

# geniusrise

**Run open LLM, STT and TTS models on infrastructure you control.**

One binary, one yaml file, one OpenAI-compatible endpoint that autoscales inside a hard budget — no kubernetes, no NAT gateways, no hosted backend.

```bash
curl -fsSL https://geniusrise.com/install.sh | sh
geniusrise init && geniusrise plan && geniusrise apply
```

<h3 align="center">
  <a href="https://docs.geniusrise.com">Docs</a>
  ||
  <a href="https://geniusrise.com">Website</a>
  ||
  <a href="https://github.com/geniusrise/geniusrise">GitHub</a>
</h3>

## What we build

| repo | what it is |
|---|---|
| [geniusrise/geniusrise](https://github.com/geniusrise/geniusrise) | the product: a single Go binary that is the CLI, the local GUI, the in-cloud gateway and the node agent |
| [geniusrise/geniusrise.com](https://github.com/geniusrise/geniusrise.com) | landing page |
| [geniusrise/docs](https://github.com/geniusrise/docs) | docs at [docs.geniusrise.com](https://docs.geniusrise.com) |

The idea: a standard IT generalist — an ISP, a community, a small company — can host open models for their people the way cable TV once distributed channels. Your `deploy.yaml` is the only state you own: a list of curated models, API keys and one budget number. GPU nodes open zero inbound ports and dial the gateway over mTLS, so homelabs behind NAT work too.

Most older repositories here are archived history from an earlier, kubernetes-flavored incarnation of the idea. The current system is a lean Go rewrite — see the [design spec](https://github.com/geniusrise/geniusrise/blob/master/docs/superpowers/specs/) and [architecture docs](https://docs.geniusrise.com/architecture/).

Apache-2.0.
