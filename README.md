# pufi-lp — лендинги Pufi VPN для рекламных кампаний

GitHub Pages: `https://deployment0987-sketch.github.io/pufi-lp/<лендинг>/`. Один лендинг — одна папка с `index.html`.

| Лендинг | Что | Адрес |
|---|---|---|
| `glushilki/` | «VPN, который работает даже при глушилках» + бесплатный перенос подписки; тёмная гамма Вады № 302 (как ролик про рефералку) | `/pufi-lp/glushilki/` |

## Параметры ссылки (одна страница служит разным кампаниям)
- `u=<utm>` — метка кампании из Hex (hexpartners.pro → Кампании): кнопка ведёт в `t.me/pufi_vpn_bot?start=utm_<utm>`,
  «Купить на сайте» — `pufi-vpn.vitrinka.net/?utm=<utm>`. На Android кнопка открывает Telegram напрямую (intent).
- `ct={{ctoken}}` — токен HilltopAds: при нажатии на кнопку страница шлёт конверсию в Hilltop (trackhta.com/close, label=click).
- остальные параметры (`s`, `z={{zoneid}}` …) страница не использует, их можно передавать для своей статистики.

Пример ссылки для HilltopAds: `https://deployment0987-sketch.github.io/pufi-lp/glushilki/?u=<utm>&z={{zoneid}}&ct={{ctoken}}`
