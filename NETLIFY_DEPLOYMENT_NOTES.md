# Netlify Deployment Notes

Use these settings in Netlify:

- Build command: `npm run build`
- Publish directory: `dist`
- Node version: `20`

This version preserves the country code `NA` as Namibia. It should not be treated as blank/missing country.

Approval ratio logic:

`Approved unique merchantOrderId / Total unique merchantOrderId`

If any transaction under the same merchantOrderId is approved, that merchantOrderId is counted as approved. Otherwise, if it has declined rows, it is counted as declined.
