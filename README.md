# IFrame Clickjacking PoC

PMSanTime doesn't send a X-Frame-Options header, allowing you to include the site on any other site using an IFrame.

Modern browsers prevent a lot of malicious attack vectors by severely limiting access to the DOM included in the IFrame. Clickjacking is the act of having a user interact with elements that are invisible or disguised as the "native" element. This PoC does a poor job of overlaying the true input elements of the "native" site, as it's not meant to be malicious, but instaed exactly as described, a proof of concept. You can increase the size of the clickjacking inputs to completely cover the "native" inputs and hide them completely from the user.
