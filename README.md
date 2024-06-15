# README

## Teste de Esparcidade Geográfica

### Dados Utilizados

Os dados utilizados fazem parte do dataset PEMSd3 e contém dados de janeiro a agosto de 2023.

Para cada tipo de teste utilizou-se apenas parte destes dados:

Interpolação: Os dados utilizados contém 1/8 do dataset original (dados de janeiro de 2023).

Esparsidade Temporal e Geográfica: Os dados utilizados contém 1/4 do dataset original (dados de janeiro e fevereiro de 2023).

### Explicações dos arquivos:

- Nas imagens geradas, os valores do eixo X representam a quantidade de sensores retirados do grafo original, por exemplo, 0.4 significa que aproximadamente 40% dos sensores do grafo original foram retirados aleatoriamente.
- Como os sensores foram retirados de forma aleatória, os grafos resultantes foram gravados em arquivos .npz, e numerados de forma correspodente.
- Além disso, cada teste foi executado usando o tensorboard e a evolução de cada treinamento também foi registrada em arquivos .csv e numerados de forma correspondente para fins de registro. Os arquivos gerados pelo tensorboard são: train_loss_{number}.csv, validation_loss_{number}.csv, train_mae_{number}.csv, validation_mae_{number}.csv, train_rmse_{number}.csv, validation_rmse_{number}.csv, train_nrmse_{number}.csv e validation_nrmse_{number}.csv. Observação: Nem todos os testes possuem esses arquivos pois alguns deles consumiram muita memória para registrar de forma simultânea essas informações.
- O arquivo data_metrics.csv contém algumas informações sobre os dados utilizados.
- O arquivo model_metrics.csv contém alguns valores sobre o modelo utilizado.
- Os arquivos metrics_training_linear.csv, metrics_validation_linear.csv e metrics_testing_linear.csv contém os resultados de cada treinamento, validação e teste.
