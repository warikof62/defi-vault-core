# 🔷 CryptoFlair

**CryptoFlair** — утилита для обнаружения "воскресших" криптокошельков, ранее долгое время не проявлявших активности (по умолчанию более 1 года).

Полезно для:

- Крипто-аналитиков
- Журналистов
- Исследователей блокчейна
- Трейдеров

## 🔍 Как это работает?

Скрипт обращается к [Etherscan API](https://etherscan.io/apis) и проверяет историю транзакций каждого адреса. Если адрес был неактивен более N дней, но недавно начал активность — это считается "воскрешением".

## 🚀 Установка

```bash
git clone https://github.com/yourusername/cryptoflair.git
cd cryptoflair
pip install -r requirements.txt
```

## 🧪 Пример запуска

```bash
python cryptoflair/watcher.py
```

## ⚙️ Настройки

В `cryptoflair/watcher.py`:

- `DAYS_INACTIVE`: кол-во дней бездействия
- `ETHERSCAN_API_KEY`: получите ключ [здесь](https://etherscan.io/myapikey)

## 📄 Лицензия

MIT
