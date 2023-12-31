# ML_Comparassion_2023

## Краткое описание
 Данный репозиторий будет содержать домашние работы по курсу "Компрессия моделей компьютерного зрения". Следуя рекомендациям преподавателям курса, была выбрана модель для экспериментов **BERT base model (uncased)**.

## Структура папок
```
|
├── README.md                           <- Этот файл Вы читаете
└── notebooks
    ├── HW1                             <- Папка домашней работы №1
    ├── ...
    └── HW7                             <- Папка домашней работы №7

```

# Темы домашних работы и ссылки
1. QUANTIZATION & PRUNING
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW1/README.md)
2. CLUSTERING
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW2/README.md)
3. DISTILLATION
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW3/README.md)
4. ONNX + OpenVINO
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW4/README.md)
5. (у нас сьехала нумерация из-за того, что сделали 1+2 домашки вместе в первой)
6. Optimum 
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW6/README.md)
7. Ускорение модели в "проде"
Ознакомиться с результатами можно по ссылке [Результаты](/notebooks/HW7/README.md), [Пулл реквест](https://github.com/aitalents/model-compression-2023/pull/11)

| Name           | device | Training | F1_test | Size(mb) | Time for 1 predict(s) |
|:----:          |:------:|:--------:|:-------:|:--------:|:---------------------:|
| Bert_orig      |  cpu   | no       |  0.629  |  438.000 | 0.8055                |
| Bert_orig      |  cuda  | yes      |  0.924  |  438.003 | 0.0356                |
| BERT_q_dynamic |  cpu   | no       |  0.543  |  181.479 | 0.6954                |
| BERT_cluster   |  cuda  | yes      |  0.589  |  438.003 | 0.0338                |
| BERT_distil    |  cuda  | yes      |  0.906  |  267.854 | 0.0182                |
| BERT_onnx      |  cpu   | yes      |  0.921  |  438.202 | 0.1309                |


P.S. Данный документ будет дополняться/наполняться по мере выполнения домашних работ.
