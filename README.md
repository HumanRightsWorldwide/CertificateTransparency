# Certificate Transparency in Chrome

## Overview

Certificate Transparency (CT) is a protocol designed to fix several structural
flaws in the SSL/TLS certificate ecosystem. Described in
[RFC 6962](https://tools.ietf.org/html/rfc6962), it provides a public,
append-only data structure that can log certificates that are issued by
[certificate authorities](https://en.wikipedia.org/wiki/Certificate_authority) (CAs).

By logging certificates, it becomes possible for the public to see what
certificates have been issued by a given CA. This allows site operators to
detect when a certificate has been issued for their domains, allowing them to
check for unauthorized issuance. It also allows browsers and root stores, and
the broader community, to examine the certificates a CA has issued and ensure
that the CA is complying with their expected or disclosed practices.

For more information about how Certificate Transparency works and its role in supporting the web PKI, you can find a helpful introduction to CT at [https://certificate.transparency.dev](https://certificate.transparency.dev/).

Chrome requires all publicly-trusted TLS certificates issued after April 30, 2018 to support CT in order to be recognized as valid. This site provides details on what is required. Any questions should be directed to the [ct-policy@chromium.org](https://groups.google.com/a/chromium.org/forum/#!forum/ct-policy) list.

## &nbsp;
