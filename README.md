# DIO - Trilha .NET - Fundamentos

## Desafio de projeto
Este repositório contém a minha solução para o desafio de projeto "Criando um sistema para um estacionamento", proposto no módulo de Fundamentos da trilha .NET da Digital Innovation One (DIO).

## Projeto
O objetivo foi construir um sistema em C# para gerenciar as operações de um estacionamento. O programa console permite:

1. Adicionar veículos
2. Remover veículos, exibindo o valor total cobrado pelo período
3. Listar todos os veículos atualmente estacionados

## Funcionalidades Implementadas
O núcleo do sistema é a classe Estacionamento, que gerencia os dados e as operações.

**Propriedades da Classe**
1. precoInicial: (decimal) Valor fixo cobrado no momento da entrada do veículo.
2. precoPorHora: (decimal) Valor cobrado por cada hora que o veículo permanece estacionado.
3. veiculos: (List<string>) Uma coleção que armazena as placas de todos os veículos presentes.

**Métodos da Classe**
1. AdicionarVeiculo: Recebe a placa digitada pelo usuário e a armazena na lista veiculos.
2. RemoverVeiculo: Método que verifica se um veículo (pela placa) está estacionado. Caso positivo, solicita ao usuário a quantidade de horas que ele permaneceu e, em seguida, calcula e exibe o valor final a ser pago.
3. ListarVeiculos: Exibe todas as placas dos veículos presentes na lista. Se o estacionamento estiver vazio, exibe a mensagem "Não há veículos estacionados".

## Menu Interativo
Para a interação com o usuário, foi implementado um menu de console que oferece as seguintes opções:
1. Cadastrar veículo
2. Remover veículo
3. Listar veículos
4. Encerrar
