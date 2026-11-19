# Vercel deployment and domain runbook

## Preview setup

1. Use the founder-created standalone repository `cbdkstan-FutureLab/ai-generation` (public visibility).
2. Connect it to the AndrewTeam Vercel account as a separate project named `ai-generation-community`; project root is the repository root and the site is static HTML with no build command.
3. Keep Vercel’s default deployment protection in place. Use pull-request or feature-branch previews for review.
4. Keep the custom domain list empty until approval is recorded against the exact Git commit.

## After founder approval

1. Record the approved commit and reviewer in the GitHub PR and `COMMUNICATION_LOG.md`.
2. Check whether `ai-generation.my` is available in the Vercel team or whether registrar/DNS access must be provided. The current Vercel team domain inventory shows `futurelab.com.my`; it does not show `ai-generation.my`.
3. Add `www.ai-generation.my` to the Vercel project and follow the exact DNS instructions returned by Vercel. Decide whether the apex `ai-generation.my` should redirect to `www` before adding it.
4. Verify the domain and TLS certificate in Vercel; then open the exact domain and confirm content, HTTPS, and preferred redirect.
5. Remove the `X-Robots-Tag: noindex, nofollow` header only in the approved public-launch change.

Domain cutover can be quick when DNS is already under the right control, but it cannot be guaranteed until registrar ownership, DNS access, and Vercel verification are confirmed.
