# V3: Требования к шифрованию

## Цель верификации

Криптография является важным компонентом защиты данных, хранящихся на мобильном устройстве. Но также это и область, в которой все может пойти не так, особенно когда стандартные соглашения не соблюдаются. Назначение верификационных требований в этой главе состоит в том, чтобы убедиться – проверенное приложение использует криптографию в соответствии с отраслевыми передовыми методами, в том числе такими, как: 

- Использование проверенных криптографических библиотек;
- Правильный выбор и настройка криптографических примитивов;
- Подходящий генератор случайных чисел везде, где требуется случайность.

## Требования к верификации безопасности

| # | Описание | L1 | L2 |
| --- | --- | --- | --- |
| **3.1** | Приложение не полагается на симметричную криптографию с жестко закодированными ключами в качестве единственного метода шифрования.| ✓ | ✓ |
| **3.2** | Приложение использует проверенные реализации криптографических примитивов. | ✓ | ✓ |
| **3.3** | Приложение использует криптографические примитивы, которые подходят для конкретного прецедента, с параметрами, которые соответствуют лучшим практикам отрасли. | ✓ | ✓|
| **3.4** | Приложение не использует криптографические протоколы или алгоритмы, которые считаются в сообществе устаревшими для целей безопасности. | ✓ | ✓|
| **3.5** | Приложение не использует один и тот же криптографический ключ для нескольких целей. | ✓ | ✓ |
| **3.6** | Все случайные значения генерируются с использованием достаточно безопасного генератора случайных чисел. | ✓ | ✓ |

## Ссылки

OWASP MSTG содержит подробные инструкции по верификации требований, перечисленных в этом разделе.

- Android - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x05e-Testing-Cryptography.md
- iOS - https://github.com/OWASP/owasp-mstg/blob/master/Document/0x06e-Testing-Cryptography.md

Для получения дополнительной информации смотрите также:

- OWASP Mobile Top 10: [M5 - Недостаточное шифрование](https://www.owasp.org/index.php/Mobile_Top_10_2016-M5-Insufficient_Cryptography)
- CWE: https://cwe.mitre.org/data/definitions/310.html
