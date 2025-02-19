# Projeto 100 | Unidade 02 | ETL | APACHE HOP | Data Analytics | Digital College Brasil

Desenvolvimento de projeto para transformar dados de um arquivo .csv num Pipeline no APACHE HOP.<br>

Instituição: [Digital College Brasil](https://digitalcollege.com.br/) (Fortaleza/CE) <br>
Curso: Data Analytics (Turma 18) <br>
Instrutora: [Nayara Wakweski](https://github.com/NayaraWakewski) <br>

## Etapas de Desenvolvimento

## 1. Step csv file input
File: cliente_veiculo.csv <br>
![screenshot](/images/csv_input_file.png) <br>
![screenshot](/images/csv_table.png) <br>

## 2. Step split fields
Tratamento da coluna dat_hora_cadastro. Separar hora e texto. <br>
![screenshot](/images/split_field_1.png) <br>
![screenshot](/images/split_field_1_table.png) <br>

## 3. Step replace in string
Tratamento da coluna des_per_tratado. Retirar texto AM. <br>
![screenshot](/images/replace.png) <br>
![screenshot](/images/replace_table.png) <br>

## 4. Novo Step replace in string
Tratamento da coluna des_per_tratado_am. Retirar texto PM. <br>
![screenshot](/images/replace_2.png) <br>
![screenshot](/images/replace_table_2.png) <br>

## 5. Step string operation
Tratamento da coluna des_per_tratado. Retirar os números. <br>
![screenshot](/images/string_operation.png) <br>
![screenshot](/images/string_operation_table.png) <br>

## 6. Step concat fields
Tratamento das colunas des_nome e des_sobrenome. Realizar o concat para formar o nome completo.<br>
![screenshot](/images/concat.png) <br>
![screenshot](/images/concat_table.png) <br>

## 7. Step string operation
Tratamento das colunas do tipo string: UPPER. <br>
![screenshot](/images/string_upper.png) <br>
![screenshot](/images/string_upper_table.png) <br>

## 8. Step if null
Tratamento das colunas com valores nulos: des_pais_origem e mod_carro. <br>
![screenshot](/images/if_null.png) <br>
![screenshot](/images/if_null_table.png) <br>

