# Changelog

## [1.1.0](https://github.com/3rd/image.nvim/compare/v1.0.0...v1.1.0) (2023-10-20)


### Features

* add editor_only_render_when_focused option ([133926c](https://github.com/3rd/image.nvim/commit/133926c01bb5160b6ff26c37891e7d8a1d73528f))
* add tmux_show_only_in_active_window option ([60d7fc6](https://github.com/3rd/image.nvim/commit/60d7fc61ff41ca9951101c245505b3a03e3eb8cb))
* auto-handle hiding/showing the images on tmux window switch ([3fbe47d](https://github.com/3rd/image.nvim/commit/3fbe47d7e1b5d18eff5fb118ee232047ac3f823d))


### Bug Fixes

* better text change handling using nvim_buf_attach ([33f7234](https://github.com/3rd/image.nvim/commit/33f72342df52af2864ec6e4a14099267cdc01b61))
* bug causing double extmark clearing weirdness ([a3e0b9f](https://github.com/3rd/image.nvim/commit/a3e0b9f0395f32d6e6c1fd8a032600ab07f8ff2b))
* clear / rerender images on BufLeave ([471eca9](https://github.com/3rd/image.nvim/commit/471eca9a895e065a16761f708ba46911987516d1))
* clear images when closing a twin window ([bd95cc9](https://github.com/3rd/image.nvim/commit/bd95cc9c13ae61b8e2453a0234250ea782b84ce7))
* commit error ([aa3004e](https://github.com/3rd/image.nvim/commit/aa3004e3e695f16166cd6c866e25a0a9ea1a51da))
* disable decoration provider handling on focus lost (when needed) ([725eccb](https://github.com/3rd/image.nvim/commit/725eccb7f50c82c9b028b3fbb461b0d2b198ef01))
* document integrations shouldn't care about resizing ([7234469](https://github.com/3rd/image.nvim/commit/7234469ce44dca9d3a3124c17daea0e9810f0ff9))
* **document:** queue images for rendering after clearing the old ones ([ae351ca](https://github.com/3rd/image.nvim/commit/ae351ca5134450b64d81e02c3d57580016b1a40b))
* **document:** rerender images when text changes in insert mode ([fb929d0](https://github.com/3rd/image.nvim/commit/fb929d0fd5a0db2983c1ad0c537e4f063ef06c45))
* guard against extmark creation errors in decoration provider ([9bf46c1](https://github.com/3rd/image.nvim/commit/9bf46c14fa1b3318e99213df5ec01272584a5010))
* plugin breaking visual mode actions and decorator optimizations ([440aee9](https://github.com/3rd/image.nvim/commit/440aee9071697b5ac1ac2e69a61c1187311c2cce))
* rendering width/height inference bug ([6e597f8](https://github.com/3rd/image.nvim/commit/6e597f84b5242e18133627c26743bcd0734de1ca))
* tmux same-window check ([2db85d0](https://github.com/3rd/image.nvim/commit/2db85d0b84dffde074622be1989a4d234b307577))

## 1.0.0 (2023-10-08)


### Features

* add "height-from-empty-lines" sizing strategy to markdown ([6412397](https://github.com/3rd/image.nvim/commit/6412397a77b34d2096372e84d751631338e24df6))
* add initial implementation for kitty unicode placeholders and debugging ([e65ca7c](https://github.com/3rd/image.nvim/commit/e65ca7c0806d9f1ecd3c7dd00c70aa3780273749))
* add Neorg integration ([069eb23](https://github.com/3rd/image.nvim/commit/069eb2372dea2273685b367d89347ec74ec772c9))
* add option to only render the image under cursor for markdown and neorg (https://github.com/3rd/image.nvim/discussions/14) ([1abfecb](https://github.com/3rd/image.nvim/commit/1abfecb67aeb103b0d597f1e8098995f2a72934d))
* add remote image support and integrate it with markdown ([7023c7d](https://github.com/3rd/image.nvim/commit/7023c7d10a78f154dc1f501c9f511aad356270ec))
* allow kitty to handle cropping in default mode for better perf ([814af48](https://github.com/3rd/image.nvim/commit/814af48b934d4f01d16f4b1f0974d495fed1b878))
* bootstrap kitty backend based on hologram.nvim ([a28df8b](https://github.com/3rd/image.nvim/commit/a28df8b844a791da3b6f9b3e824886f88bf692b5))
* cache intermediary converted, resized, and cropped image variants ([961e5a6](https://github.com/3rd/image.nvim/commit/961e5a68998dd76bf5e25ae2d96fcf3bb1ee22ae))
* compute window masks and toggle overlapped window images ([e524050](https://github.com/3rd/image.nvim/commit/e5240500b82cfc396bfd7e975da3cd3bd5f763b9))
* export basic rendering operations render() and clear() ([4515796](https://github.com/3rd/image.nvim/commit/4515796c3bdcb2e9369aee0ca0ea39027f7b742b))
* extract cropping into renderer and handle with magick ([573e057](https://github.com/3rd/image.nvim/commit/573e0575313c14558be08db72a02b1b29f3ad73d))
* genesis ([16d34a0](https://github.com/3rd/image.nvim/commit/16d34a049d894beacbbd8a2770c1831c248ecc17))
* handle bounds separately in backends, multi-split support ([c45a050](https://github.com/3rd/image.nvim/commit/c45a0504cafe38ff98004e76c046c1c1e286908f))
* handle extmark scroll, allow editing and preview in markdown at the same time, fix kitty clear ([31d12e0](https://github.com/3rd/image.nvim/commit/31d12e0210a51ff9f0e38ae2fd5cf74ac3ff7088))
* handle folds ([e42ea8c](https://github.com/3rd/image.nvim/commit/e42ea8c032b368aaf826c5c32498dbb86e22d1be))
* kitty vertical split bottom crop ([445fc24](https://github.com/3rd/image.nvim/commit/445fc24557d07361fac4338419e075845f121d9f))
* markdown - add clear_in_insert_mode option ([c4d14a2](https://github.com/3rd/image.nvim/commit/c4d14a2a5efc17d7c7f6afc12f27872de2d254a3))
* markdown - add toggle for remote image downloads ([dbf1f15](https://github.com/3rd/image.nvim/commit/dbf1f1521560bc20f8e89f6f418622d26fd7b260))
* markdown - resolve relative images ([dd93b11](https://github.com/3rd/image.nvim/commit/dd93b11164f046b0570c461b82de4d890804499a))
* move to imagemagick for image handling ([3dbb7f4](https://github.com/3rd/image.nvim/commit/3dbb7f45be8af7071cf24ad20d2f56b04ae74d0d))
* remote url support for neorg (images must be alone on lines and start with .image) ([7f2edec](https://github.com/3rd/image.nvim/commit/7f2edec4c11f24529b8124ce49bdae3a9969e6bd))
* rework image API and add support for magick manipulations ([4fbc195](https://github.com/3rd/image.nvim/commit/4fbc1951c45756116bf003fcfbfb8e2b5478c3c3))
* rewrite most things, restructure API, extmarks, multi-window support, auto-clear,  ueberzug++ ([cd58741](https://github.com/3rd/image.nvim/commit/cd587411c85d1e11d1c871748bf5f14e9d5a5940))
* scale down big images before rendering instead of cropping right and fix rendering bug ([6972ff4](https://github.com/3rd/image.nvim/commit/6972ff44ed784921fda0f1706ba1fae61051ea8e))
* tmux + kitty (normal) rendering ([4399f69](https://github.com/3rd/image.nvim/commit/4399f69043df82cc491168b0260d9c071aab4682))
* use atomic screen updates for kitty ([6623c7e](https://github.com/3rd/image.nvim/commit/6623c7e314579cc5e6ff98472757e29e75491019))
* window-relative rendering, refactor general structure, types, many things ([2134ca7](https://github.com/3rd/image.nvim/commit/2134ca79a6af8aa7ab97719acf6d841f5b008b75))


### Bug Fixes

* add url to image id ([2c1e1a6](https://github.com/3rd/image.nvim/commit/2c1e1a6b79b9759a873bf5189e4c1ae937a53d2e))
* bail early when checking for images to clear if there are no images ([c891ad8](https://github.com/3rd/image.nvim/commit/c891ad866045cba6fc84dd22423589ce3d7e798a))
* bottom cropping ([90c5183](https://github.com/3rd/image.nvim/commit/90c51839a0bf05a209b78fa2b6858228e800b3e9))
* cache TIOCGWINSZ ([847f5d6](https://github.com/3rd/image.nvim/commit/847f5d6d37f0607a29485944768ff3ff6a6b1952))
* check for ft in markdown autocommands ([9aa67f6](https://github.com/3rd/image.nvim/commit/9aa67f6582f6384b3b18cfeeb83ce52888bb8d29))
* check that window and buffer are valid & init namespace directly ([ef15a6d](https://github.com/3rd/image.nvim/commit/ef15a6d5f2e93b635dcddf4de1f76c706e3f4d0f))
* clear images even if they're not rendered ([ddf4b58](https://github.com/3rd/image.nvim/commit/ddf4b58bec33b46d319ee1392382982777a08ffb))
* clear images on window close ([692bcb7](https://github.com/3rd/image.nvim/commit/692bcb7bb1ed29f9c8b7b8524f150180b10f6cf1))
* destroy magick image after crop ([8f7a054](https://github.com/3rd/image.nvim/commit/8f7a054bafa97eb0e77774a9e11c3d0e2d0b01fb))
* don't fetch images in insert mode ([16f5407](https://github.com/3rd/image.nvim/commit/16f54077ca91fa8c4d1239cc3c1b6663dd169092))
* don't wrap backend and integration load errors ([ae0bbc4](https://github.com/3rd/image.nvim/commit/ae0bbc408bddf022689c2239c43ef65c8863e802))
* fix images not working if initially inside folds & extmark tweaks ([03f4eb7](https://github.com/3rd/image.nvim/commit/03f4eb748e311aaf3af7f8bb2211c60b59160963))
* handle folds when having less lines than window height ([d2a69cd](https://github.com/3rd/image.nvim/commit/d2a69cd4222297d32671d69f27fd6722688d3646))
* handle images with zero width/height ([e4d3c4c](https://github.com/3rd/image.nvim/commit/e4d3c4c405f96975bcf89997c068f1d0ce9115cb))
* increase default tmux write delay ([b8b9633](https://github.com/3rd/image.nvim/commit/b8b9633c6fc5c5e40360ff615bfbb55d84c5a537))
* kitty - clear images on exit ([2561f01](https://github.com/3rd/image.nvim/commit/2561f01bcf44c6f4014c7c92da3225f78fda0c44))
* kitty - re-transmit images after vim resize ([3037f1d](https://github.com/3rd/image.nvim/commit/3037f1d2d8f004d69b421bf1f2267e55f2ac975b))
* kitty - save some cursor movements ([11a5452](https://github.com/3rd/image.nvim/commit/11a54524b9e0611f2646bb41cd38b7c12096118e))
* leftover ([8f03d32](https://github.com/3rd/image.nvim/commit/8f03d32aa75f3ad4f0262320024092fb326f58d6))
* markdown - follow clear_in_insert_mode when editing in insert mode ([a15734e](https://github.com/3rd/image.nvim/commit/a15734e70bf66e920223656d835a37e1cb44f822))
* markdown - ignore loading errors ([dec5c4c](https://github.com/3rd/image.nvim/commit/dec5c4c8a8d3355798ba65bc35f8e0c20d4794e9))
* only cache remote image urls, fixes same remote image in multiple splits ([1738f08](https://github.com/3rd/image.nvim/commit/1738f08e14730074d25d29eaf0c19882218d1b08))
* optimize kitty rendering (non-cropped) ([52b25c3](https://github.com/3rd/image.nvim/commit/52b25c375ed14de3948d4ff522705eeb0ee4d3df))
* prevent unnecessary rerenders ([c7d977c](https://github.com/3rd/image.nvim/commit/c7d977c6b4e2db5d76baf60fd7020f71a66f1a40))
* prevent unnecessary rerenders and recrop previous images on new splits ([b2ac03f](https://github.com/3rd/image.nvim/commit/b2ac03f352958c009534b5c6b9f12b3a9c51793a))
* prevent useless rerenders and clean-up ([4d1ab88](https://github.com/3rd/image.nvim/commit/4d1ab88049ca1dae47765a0c36131d6037ceb8a6))
* remove extmark map entry when clearing image ([4a68eda](https://github.com/3rd/image.nvim/commit/4a68eda54ef695f6ec025f874f67e9958ddff1b8))
* remove tmux cursor delay and silence winclosed error ([0b2dae8](https://github.com/3rd/image.nvim/commit/0b2dae85a5150a13b7f2ef7a4b20bf8faa6dea07))
* rendering errors when geometry is not provided, limit vspace y ([b6057c5](https://github.com/3rd/image.nvim/commit/b6057c5022a08e3ed37b6d8c26be63661d1cc482))
* rendering glitches and handle buffer change clearing through decoration provider ([5979f47](https://github.com/3rd/image.nvim/commit/5979f47e0510d266acbe838415f994d53497662b))
* replace '/' with '-' in base64 encode ([1e0a270](https://github.com/3rd/image.nvim/commit/1e0a27024f19c5e1f5307c449380f54888301c5e))
* rerender affected images after updating extmarks ([b5e8b75](https://github.com/3rd/image.nvim/commit/b5e8b756d0bcc4756e41684667c541cd3afd6c7f))
* rerender images below the current one after adding extmark ([093ef13](https://github.com/3rd/image.nvim/commit/093ef13a4f9920fd7a78f83b7b6dcf9b8cb672b3))
* restore winscrolled handling ([721bc43](https://github.com/3rd/image.nvim/commit/721bc43fe13287e9745903740cb6c5d9da8e0b76))
* track and reset crop, fix vertical screen bounds ([affcc53](https://github.com/3rd/image.nvim/commit/affcc53023bcc784a98f1daa945f1898f4a0a8c2))
* ueberzug - prevent useless clear ([bffa411](https://github.com/3rd/image.nvim/commit/bffa41142dce95c20fefa45809c13c9d9c4e9925))
* update kitty backend to the new structure ([3ca9bf5](https://github.com/3rd/image.nvim/commit/3ca9bf5bd4651d4451d121f1e538ad2fa46ef126))
* wrong positioning, window/gutter offset math, ty https://github.com/3rd/image.nvim/pull/6 ([c957678](https://github.com/3rd/image.nvim/commit/c9576783d2eac3594fc6d264001e10bec60444b9))


### Performance Improvements

* optimize rendering and always use shallow delete for kitty images ([05679fa](https://github.com/3rd/image.nvim/commit/05679faad71bb0dd6475b539657d02c5dd6e3322))
* re-use fixed paths for source, resized, and cropped image variants ([7a98960](https://github.com/3rd/image.nvim/commit/7a98960aace23bf845b39b89d64f52f26bec01c1))
* split pre-processing caching into resize and crop ([d3b3246](https://github.com/3rd/image.nvim/commit/d3b32462e252f448c994ba291c1e741df3bebabb))
