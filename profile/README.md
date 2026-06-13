# speedata

We build software for **automated, high-quality typesetting** — turning structured
data (XML, JSON, databases) into beautifully laid out PDFs. Catalogs, data sheets,
price lists, reports, invoices: anything where layout matters and the content keeps
changing.

Most of what you'll find on this page exists because we needed it ourselves while
building our main product, the **speedata Publisher**. We open-sourced the pieces
that we thought others might find useful too.

> **Looking for the big picture?** [**constellation.speedata.de**](https://constellation.speedata.de)
> is an interactive map of all our open source projects around PDF, typesetting and
> publishing — showing how the pieces below fit together.

---

## speedata Publisher

A professional database publishing system. You give it your data and a layout
description, it gives you a print-ready PDF — fully scriptable, reproducible, and
suitable for very long and very demanding documents.

- Repository: [publisher](https://github.com/speedata/publisher)
- Examples: [examples](https://github.com/speedata/examples)
- Documentation & downloads: <https://www.speedata.de>

The Publisher is free and open source (AGPLv3). We also offer **commercial
licenses, training and support contracts** for teams that need guarantees,
priority fixes or help getting their first project into production — that is how
we fund the work you see here. If that sounds relevant, [get in
touch](https://www.speedata.de/en/contact/).

## XTS — the next-generation typesetting system

[xts](https://github.com/speedata/xts) is our experimental successor: a smaller,
more modern XML typesetting engine that incorporates everything we have learned
from years of running the Publisher in production. Still evolving, but already
usable — see [xts-examples](https://github.com/speedata/xts-examples) for what
it can do today.

## XML, XPath and XSLT for Go

Working with XML in Go is famously thin on the ground. While building the
Publisher we ended up writing a small ecosystem of XML tools that we now use
everywhere — and that you can use independently in your own projects:

- **[goxml](https://github.com/speedata/goxml)** — a struct-based XML
  representation for Go that preserves enough of the original document to
  round-trip cleanly.
- **[goxpath](https://github.com/speedata/goxpath)** — a full XPath 3.1
  interpreter for Go. As far as we know, the most complete one in the ecosystem.
- **[goxslt](https://github.com/speedata/goxslt)** — an XSLT processor written in
  pure Go, no libxslt required.

If you arrived here from one of these libraries: hi! They are battle-tested
because we use them ourselves, every day, inside the Publisher.

## Tools around the Publisher

- **[imageshaper](https://github.com/speedata/imageshaper)** — generates outline
  paths for images, used for text-around-image effects.
- **[vscode-speedata](https://github.com/speedata/vscode-speedata)** — a VS Code
  extension for editing RelaxNG-validated XML, including the Publisher's layout
  language.
- **[einvoice](https://github.com/speedata/einvoice)** — a Go library for
  reading and writing electronic invoices (ZUGFeRD / Factur-X / XRechnung).

## Forks and contributions

We also maintain a few forks of upstream projects with patches that matter to us
(`css`, `barcode`, `go-lua`). Most of these track upstream loosely; have a look
at the individual repositories if you need details.

---

## Get in touch

- Website: <https://www.speedata.de>
- Documentation: <https://doc.speedata.de>
- Commercial support, training, custom development:
  <https://www.speedata.de/en/contact/>

Based in Berlin, working with publishers, agencies and in-house teams worldwide.
