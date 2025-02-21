# Projeto 100 | Unidade 02 | ETL | APACHE HOP | Data Analytics | Digital College Brasil

Desenvolvimento de projeto para transformar dados de um arquivo .csv através da ferramenta APACHE HOP (Pipeline). Output: Arquivo tratado disponível em diretório do usuário.<br>

Instituição: [Digital College Brasil](https://digitalcollege.com.br/) (Fortaleza/CE) <br>
Curso: Data Analytics (Turma 18) <br>
Instrutora: [Nayara Wakweski](https://github.com/NayaraWakewski) <br>

## Pipeline Final
![screenshot](/images/pipeline.png) <br>

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

## 7. Novo Step string operation
Tratamento das colunas do tipo string: UPPER. <br>
![screenshot](/images/string_upper.png) <br>
![screenshot](/images/string_upper_table.png) <br>

## 8. Step if null
Tratamento das colunas com valores nulos: des_pais_origem e mod_carro. <br>
![screenshot](/images/if_null.png) <br>
![screenshot](/images/if_null_table.png) <br>

## 9. Step if null
Tratamento das colunas com valores nulos: des_pais_origem e mod_carro. <br>
![screenshot](/images/if_null.png) <br>
![screenshot](/images/if_null_table.png) <br>

## 10. Step value mapper
A partir da coluna des_pais_origem, criar coluna des_continente. Ex.: Para país BRAZIL, continente será AMERICA DO SUL.<br>
![screenshot](/images/value_mapper.png) <br>
![screenshot](/images/value_mapper_table.png) <br>

## 11. Step number range
A partir da coluna ano_carro, definir o status do carro entre: VELHO, CONSERVADO, NOVO.<br>
![screenshot](/images/number_range.png) <br>
![screenshot](/images/number_range_table.png) <br>

## 12. Step select values
Etapa para ordenar colunas e excluir colunas não necessárias para o output.<br>
![screenshot](/images/select_values.png) <br>
![screenshot](/images/select_values_table.png) <br>