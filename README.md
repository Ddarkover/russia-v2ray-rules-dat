# Об этом репозитории

Здесь публикуются автоматически обновляемые файлы маршрутизации (`geoip.dat` и `geosite.dat`) для **V2Ray** и совместимых прокси-инструментов.  
В их основе — данные о заблокированных доменах и IP-адресах на территории РФ.

✅ Поддерживаются: [V2Ray](https://github.com/v2fly/v2ray-core), [v2rayN](https://github.com/2dust/v2rayN), [Xray-core](https://github.com/XTLS/Xray-core), [mihomo](https://github.com/MetaCubeX/mihomo/tree/Meta), [hysteria](https://github.com/apernet/hysteria), [Trojan-Go](https://github.com/p4gefau1t/trojan-go), [leaf](https://github.com/eycorsican/leaf) и другие.

🔄 Частота обновления: **каждые 6 часов**.

---

## Состав и категории

### geoip.dat

Генерируется из репозитория [@Ddarkover/russia-blocked-geoip](https://github.com/Ddarkover/russia-blocked-geoip)

**Основные блоки:**
- `ru-blocked` — на основе `ipresolve.lst` и `subnet.lst` от antifilter.download  
- `ru-blocked-community` — на основе `community.lst` (community.antifilter.download)  
- `re-filter` — на основе `ipsum.lst` из [re:filter](https://github.com/1andrevich/Re-filter-lists)

**Дополнительные категории (по ASN):**
`cloudflare`, `cloudfront`, `facebook`, `fastly`, `google`, `netflix`, `telegram`, `twitter`, `ddos-guard`, `yandex`

**Добавленные вручную (по ASN):**
`network-solutions`, `wpengine`, `hostgator`, `ionos`, `dreamhost`, `aws`, `godaddy`, `bluehost`, `kamatera`, `ovh`, `hetzner`, `digitalocean`, `akamai`, `vultr`, `scaleway`, `cdn77`

### geosite.dat

Генерируется из репозитория [@Ddarkover/russia-blocked-geosite](https://github.com/Ddarkover/russia-blocked-geosite)

**Доступные категории:**
- Все из [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community/tree/master/data): `google`, `discord`, `youtube`, `twitter`, `meta`, `openai` и др.
- `ru-blocked` — заблокированные в РФ домены (`antifilter-download-community` + `re:filter`)
- `ru-blocked-all` — **все известные** заблокированные домены РФ (≥700 тыс., использовать осторожно)
- `ru-available-only-inside` — домены, доступные только внутри РФ
- `antifilter-download` — все домены из antifilter.download (~700 тыс., с осторожностью)
- `antifilter-download-community` — домены из community.antifilter.download
- `refilter` — домены из re:filter
- `category-ads-all` — рекламные домены
- `win-spy` — телеметрия и аналитика Windows
- `win-update` — обновления Windows
- `win-extra` — прочие домены Windows

---

## Скачать (последняя версия)

- **geoip.dat**  
  [https://raw.githubusercontent.com/Ddarkover/russia-v2ray-rules-dat/release/geoip.dat](https://raw.githubusercontent.com/Ddarkover/russia-v2ray-rules-dat/release/geoip.dat)

- **geosite.dat**  
  [https://raw.githubusercontent.com/Ddarkover/russia-v2ray-rules-dat/release/geosite.dat](https://raw.githubusercontent.com/Ddarkover/russia-v2ray-rules-dat/release/geosite.dat)

---

## Связанные проекты

- [russia-blocked-geoip](https://github.com/Ddarkover/russia-blocked-geoip) — генерация geoip  
- [russia-blocked-geosite](https://github.com/Ddarkover/russia-blocked-geosite) — генерация geosite  
- [russia-v2ray-custom-routing-list](https://github.com/Ddarkover/russia-v2ray-custom-routing-list) — готовые правила маршрутизации  
- [geodat2srs](https://github.com/Ddarkover/geodat2srs) — конвертер geoip/geosite.dat → sing-box srs

---

## Благодарности

- [antifilter.download](https://antifilter.download/) — данные о блокировках и сообщество  
- [re:filter](https://github.com/1andrevich/Re-filter-lists) — отфильтрованные списки блокировок  
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) — идея и основа проекта
