Demos Ra
========

I build plain-text data tools for AI agents and the people who work with
them. Every one rests on Multi-Sheet Tab-Separated Values (MTSV), a file
format registered as an IETF Internet-Draft: TSV with one more dimension,
where a tab separates fields, a line break separates records, and a form
feed separates sheets. A whole Excel (XLSX) workbook becomes one text file
that any AI agent, editor or script can read.

Why It Is Useful
----------------

AI agents read text. Excel workbooks, databases and agent memory are
usually binary or locked inside one tool, so an agent cannot see them whole.
MTSV keeps every sheet in plain text, so people, AI agents and ordinary
tools all read and change the same file.

Repositories
------------

* [mtsv-spec](https://github.com/demos-ra/mtsv-spec): the MTSV specification, an IETF Internet-Draft
  * [mtsv](https://github.com/demos-ra/mtsv): Python library and command that convert Excel, ODS, CSV, JSON, SQLite, Parquet and Arrow to and from MTSV
    * [mtsv-office](https://github.com/demos-ra/mtsv-office): open and save spreadsheets as MTSV in office apps: LibreOffice Calc now, Excel next
    * [text-spreadsheet](https://github.com/demos-ra/text-spreadsheet): MCP (Model Context Protocol) server that lets AI agents read Excel, CSV and other spreadsheets as text
    * [living-memory](https://github.com/demos-ra/living-memory): agent memory for any AI agent, as plain tables; Claude Code first
  * [living-architecture](https://github.com/demos-ra/living-architecture): code generation from small MTSV grids, for Next.js, TypeScript, React, Prisma, CSS and JSON
  * [void-os](https://github.com/demos-ra/void-os): the personal operating system for AI agents: memory, tools and hooks in one relational data bank of plain text

Linux Kernel
------------

* [457dc9fefe9a ("netlink: specs: Add a spec for nexthops in rtnetlink")](https://git.kernel.org/netdev/net-next/c/457dc9fefe9a): a YNL spec for nexthop objects and nexthop buckets in rtnetlink, applied to net-next by Jakub Kicinski in October 2026; [the patch on the netdev mailing list](https://lore.kernel.org/20261019-rt-nexthop-spec-v1-1-9c586edf86ab@gmail.com)

Get Started
-----------

* [Convert Excel and other files to MTSV](https://github.com/demos-ra/mtsv): `pipx install mtsv`
* [Let AI agents read Excel through an MCP server](https://github.com/demos-ra/text-spreadsheet): `pipx install text-spreadsheet`
* [Run the operating system for AI agents](https://github.com/demos-ra/void-os): `pipx install void-os` or `npm install --global void-os`

Get Help
--------

* Issues: the issue tracker of each repository
* Maintainer: Demos Ra
