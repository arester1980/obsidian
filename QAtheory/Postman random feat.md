Бывает, что нужно добавить случайные данные в наш URL или тело запроса.  
Чтобы избежать спамминга одинаковыми вызовами, их можно рандомизировать при помощи динамических переменных, предоставляемых Postman
```
{{$randomAlphaNumeric}}
```
  
Или можно загружать данные из JSON или CSV-файла, в каждой итерации создавая переменную на основе следующего массива/строки. Но в нашем примере этот шаг не нужен.

[Source](https://testengineer.ru/testirovanie-proizvoditelnosti-v-postman/ "https://testengineer.ru/testirovanie-proizvoditelnosti-v-postman/")
