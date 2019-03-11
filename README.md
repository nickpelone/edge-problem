# How to reproduce:

- `polymer build` to produce the minified bundle.
- `python -m http.server 8080` to start a normal webserver
  * This is to avoid any `polymer serve` rewrite magic
- Go to the launched server in Microsoft Edge
- See in the console that the bundle could not be understood, with the cryptic:
  `SCRIPT5022: SCRIPT5022: Expected identifier, string or number` at source location `(1,1)`,
  which is obviously wrong.