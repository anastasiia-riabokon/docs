```
let status = null;
console.log(typeof status); // виведе "object"
```

`null` насправді є примітивним значенням, а не об'єктом.

Коли ми використовуємо оператор `typeof` для перевірки типу значення `null`, він повертає рядок `object`. Це може здатися дивним, оскільки `null` — це фактично відсутність значення, а не об'єкт.

*Причина цього полягає в тому, що в ранніх версіях JavaScript `null` було розглянуто як спеціальний випадок об’єкта. Це була помилка в реалізації мови, збережена для забезпечення зворотної сумісності з існуючим кодом. Тому коли typeof застосовується до `null`, він повертає `object`, щоб зберегти цю сумісність.*