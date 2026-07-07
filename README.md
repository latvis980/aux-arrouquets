# Aux Arrouquets — A Medieval Estate in Gascony

A private, password-protected landing page for the sale of **Aux Arrouquets**,
a medieval Bastide estate in the Golden Triangle of the Gers, L'Occitanie,
Southwest France.

## Access

The page is protected. Visitors are shown a password prompt; the correct
password decrypts and displays the page in the browser. The password is shared
privately — it is **not** stored in this repository.

## How the protection works

`index.html` contains only the **encrypted** page. The full content (text and
all embedded photography) is encrypted with **AES-256-GCM**, using a key derived
from the password via **PBKDF2-SHA256**. Decryption happens entirely in the
browser using the built-in Web Crypto API — there are no external dependencies
and no server. Without the correct password, the repository and page source
contain only unreadable ciphertext.

## View it live

Once GitHub Pages is enabled (Settings → Pages → Deploy from a branch →
`main` / root):

**https://latvis980.github.io/aux-arrouquets/**

## Contact

Enquiries: auxarrouquets.france@gmail.com
