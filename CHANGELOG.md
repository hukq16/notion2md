<!--next-version-placeholder-->

## v2.3.2 (2022-01-22)
### Fix
* Merge error ([`a4244c0`](https://github.com/echo724/notion2md/commit/a4244c0064db5deb797ad64953f8ab07e5fb5d6b))
* Change directory of downloaded files ([`452cc69`](https://github.com/echo724/notion2md/commit/452cc69f56972ee15b721ffda19a3c39ac404bd8))

### Documentation
* Change Contribution guide in README.md ([`2c2c1da`](https://github.com/echo724/notion2md/commit/2c2c1daef50127995384dde4df57b21d789ca653))
* Add CONTRIBUTE.md ([`18be264`](https://github.com/echo724/notion2md/commit/18be264b4ed41eaee9c76f59f200714e47772bac))

## v2.3.1 (2022-01-17)
### Fix
* Key error ([`af224a6`](https://github.com/echo724/notion2md/commit/af224a62580551df3e2c49aa361c359175dd9eea))

## v2.3.0 (2022-01-17)
### Feature
* Add file(image) downloader #20 ([`d42a1a0`](https://github.com/echo724/notion2md/commit/d42a1a02975181b05d9290f12adc3f7bc2b87c51))

## v2.2.8 (2022-01-11)
### Fix
* Fix name of image in block converter ([`757e253`](https://github.com/echo724/notion2md/commit/757e2534a55eafa9041d0f24b340504f09f92892))

## v2.2.7 (2022-01-11)
### Fix
* Add handling 'mention' object to fix #18 ([`291b2c1`](https://github.com/echo724/notion2md/commit/291b2c1867d766e996168c6157dabf8ba25f9c03))
* Change ERROR color to RED ([`1ac9c80`](https://github.com/echo724/notion2md/commit/1ac9c8013c247b132743795ed1260027d4067c63))

## v2.2.6 (2022-01-11)
### Documentation
* Update README.md ([`ff115cb`](https://github.com/echo724/notion2md/commit/ff115cb091520843eaa18cf691e147db076e8fc0))

## v2.2.5 (2021-12-21)
### Fix
* Unpacking config dick error ([`6d0b105`](https://github.com/echo724/notion2md/commit/6d0b105c05ab12671d930dd61e72f7014985bb09))

## v2.2.4 (2021-12-21)
### Fix
* Format console output ([`bf27ced`](https://github.com/echo724/notion2md/commit/bf27ced9eed5dfa173331a53aa76c9dd52f05499))
* Refactorize exporter ([`661e3f8`](https://github.com/echo724/notion2md/commit/661e3f85e432674adbf2009fd0165af4e02cb543))
* Add checking version ([`2c9a6c1`](https://github.com/echo724/notion2md/commit/2c9a6c19ff96bfd8ba3073e49f87e5c04fa8edb6))
* Change file name as id because title can cause dir error ([`4db6e0f`](https://github.com/echo724/notion2md/commit/4db6e0f37421d092099929910d5bcbaa7831d332))
* Halt program after token error catched ([`0c356b4`](https://github.com/echo724/notion2md/commit/0c356b4c3e772cb059e3a9fb7321878a89ed0b60))

## v2.2.3 (2021-12-18)
### Fix
* Showing error message when client didn't get client ([`3e07428`](https://github.com/echo724/notion2md/commit/3e07428c96adc37a70c8fcd9cda70dae59873656))

## v2.2.2 (2021-12-16)
### Fix
* Fix script not working ([`e001e75`](https://github.com/echo724/notion2md/commit/e001e75eb8cd7c19f702510008e872cec9e7a331))

## v2.2.1 (2021-12-16)
### Fix
* Fix module names ([`e323911`](https://github.com/echo724/notion2md/commit/e3239110f8a72fd337b58ba2221b0df136f8c6a1))

# Update v2.2

- Stylized terminal output

# Update v2.1

- Improved exporting speed by using MultiThreading

# v2.0

- Notion Markdown Exporter(notion2md) now use **official notion api** by [notion-sdk-py](https://github.com/ramnes/notion-sdk-py)

- Rewrite the structure of the program to use the api and improve the speed and usability of API

## v1.2.2.1

- Supports **Inline Math Code** in the `text block`, `bulleted list`, and `numbered list`. It will Be denoted as `$$<math code>$$`

- Supports Call `export_cli()` with `token_v2`, `url`, and `bmode`

# v1.2.0

- Now Supports Exporting the **inline table block**
    
    - Even the block that has its own page in the table will be exported as **subpage**

- You can choose wheather you will export notion page as `a blog post` or not

    - Blog post format includes frontmatter and Date in Post's name.

# v1.1.0

- Change the output folder name `Notion_Exporter_Output/` to `notion_output/`

- Save token_v2 in `notion_output/notion_token.json` and read it when you use the exporter again.

- Fix the error that `block.icon` is not defined if the block has no icon in the title.

# v1.0.0

- Changed the structure of the exporter to support exporting sub pages and sub files.

- Used Object named '`PageBlockExporter`' to connect supporting functions and attributes.

- Each Exporter has its client(`NotionClient`), page(`notion.Block`), and sub pages' exporter list (`[PageBlockExporter]`)
