<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

A na-atụ aro ka ịwụnye nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mbụ, wee `direnv allow` ka mgbe ịbanye na ndekọ ( [a ga-egbu .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) na-akpaghị aka mgbe ịbanye na ndekọ).

Ọ pụtara bụ: Ntụgharị asụsụ Chinese gaa na Japanese, Korean, English, English n'asụsụ ndị ọzọ niile. Ọ bụrụ na ịchọrọ ịkwado Chinese na Bekee, ị nwere ike dee `zh: en` .

## koodu n'ihu

* [koodu n'ihu](https://github.com/xxai-art/web)
* [Nchịkọta asụsụ maka saịtị ahụ n'ozuzu ya](https://github.com/xxai-art/web/tree/main/i18n)
* [Ngwungwu asụsụ maka modul nbanye](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Weebụsaịtị akwụkwọ ọtụtụ asụsụ](https://github.com/xxai-doc)

Asụsụ mmemme mmemme n'ihu bụ [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , nke na-agbakwunye ụfọdụ atụmatụ dabere na syntax coffeescript, lee [./coffee_plus.md](./coffee_plus.md) .

## Internationalization nke weebụsaịtị na akwụkwọ

Mee na oru 3 ndị a

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Suffix bụ `.mdt` , ị nwere ike iji syntax yiri `<+ ./coffee_plus/import.js>` iji zoo aka na faịlụ mpụga, wee mepụta akara akara na suffix `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Ntụgharị asụsụ Markdown agaghị atụgharị asụsụ koodu na njikọ, ma ga-echekwa ahịrịokwu atụgharịrị. Ọ bụrụ na agbanwegharịrị ntụgharị asụsụ mana emezighị ederede izizi, ime ya ọzọ agaghị edegharị mgbanwe ntụgharị asụsụ ahụ.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Faịlụ asụsụ maka ịtụgharị `yaml` webụsaịtị ewepụtara.

### Ntuziaka akpaaka ntụgharị akwụkwọ

Hụ ebe nchekwa koodu [xxai-art/doc](https://github.com/xxai-art/doc)

A na-atụ aro ka ịwụnye nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mbụ, wee `direnv allow` ka mgbe ịbanye na ndekọ ( [a ga-egbu .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) na-akpaghị aka mgbe ịbanye na ndekọ).

Iji zere nnukwu koodu ntọala sụgharịa n'ọtụtụ narị asụsụ, m mepụtara ntọala koodu dị iche iche maka asụsụ ọ bụla wee mepụta nzukọ iji chekwaa ntọala koodu.

Ịtọ ntọala gburugburu `GITHUB_ACCESS_TOKEN` na-agba ọsọ [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) ga-emepụta koodu nchekwa ozugbo.

N'ezie, ị nwekwara ike itinye ya na ntọala koodu.

Ntuziaka ederede ntụgharị [ọsọ.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

A tụgharịrị koodu edemede ahụ dịka ndị a:

[bunx](https://bun.sh/docs/cli/bunx) bụ nnọchi npx, nke na-adị ngwa ngwa. N'ezie, ọ bụrụ na itinyeghị bun, ị nwere ike iji `npx` kama.

`bunx mdt zh` renders `.mdt` na ndekọ aha zh ka `.md` , lee faịlụ 2 jikọtara n'okpuru

* [kọfị_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [kọfị_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` bụ koodu bụ isi maka ntụgharị asụsụ (ọ bụrụ na etinyere `nodejs` naanị, mana etinyeghị `bun` na `direnv` , ị nwekwara ike ịgba `npx i18n` iji tụgharịa asụsụ).

Ọ ga-atụgharị [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , nhazi nke `i18n.yml` na akwụkwọ a bụ nke a:

```
en:
zh: ja ko en
```

Ọ pụtara bụ: Ntụgharị asụsụ Chinese gaa na Japanese, Korean, English, English n'asụsụ ndị ọzọ niile. Ọ bụrụ na ịchọrọ ịkwado Chinese na Bekee, ị nwere ike dee `zh: en` .

Nke ikpeazụ bụ [gen.README.kọfị](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , nke na-ewepụta ọdịnaya dị n'etiti isi aha na ndepụta okwu mbụ nke asụsụ ọ bụla `README.md` iji mepụta ntinye `README.md` . Koodu dị nnọọ mfe, ị nwere ike ile ya n'onwe gị.

A na-eji Google API maka ntụgharị asụsụ efu. Ọ bụrụ na ịnweghị ike ịnweta Google, biko hazie ma tọọ proxy, dịka:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Ederede ntụgharị asụsụ ga-ewepụta cache atụgharịrị na ndekọ ndekọ `.i18n` , biko jiri `git status` lelee ya wee tinye ya na ebe nchekwa koodu ka ịzena ntụgharị asụsụ ugboro ugboro.

Biko na-agba ọsọ `bunx i18n` oge ọ bụla ị megharịrị ntụgharị asụsụ iji melite cache.

Ọ bụrụ na gbanwetụrụ ederede mbụ na ntụgharị asụsụ n'otu oge, cache ga-agbagwoju anya, yabụ ọ bụrụ na ịchọrọ ịgbanwe, ị nwere ike gbanwee naanị otu, wee mee `bunx i18n` ka imelite cache.
