# Calculo de Diferença de Datas

Este projeto contém uma classe em Python que calcula a diferença em dias entre duas datas fornecidas.

Classe CalculoDiferencaDatas

# Descrição:
A classe CalculoDiferencaDatas recebe duas datas no formato YYYY-MM-DD e calcula a diferença em dias entre elas.

# Métodos

__init__(self, data1, data2): Construtor que inicializa as datas.
calcular_diferenca(self): Método que calcula e retorna a diferença em dias entre data1 e data2.

# Exemplo de Uso

from datetime import datetime

class CalculoDiferencaDatas:
    def __init__(self, data1, data2):
        self.data1 = datetime.strptime(data1, "%Y-%m-%d")
        self.data2 = datetime.strptime(data2, "%Y-%m-%d")

    def calcular_diferenca(self):
        diferenca = self.data2 - self.data1
        return diferenca.days

data_inicial = "2024-01-01"
data_final = "2024-03-01"
calculadora = CalculoDiferencaDatas(data_inicial, data_final)
print("Diferença entre as datas:", calculadora.calcular_diferenca(), "dias")

# Saída Esperada

Diferença entre as datas: 60 dias

# Requisitos

Python 3.x

# Como Executar

1. Certifique-se de ter o Python 3.x instalado em sua máquina.
2. Copie o código fornecido em um arquivo com extensão .py, por exemplo, calculo_diferenca_datas.py.
3. Execute o arquivo usando o comando python calculo_diferenca_datas.py.
