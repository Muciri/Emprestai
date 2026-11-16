# Emprestaí

Emprestaí é um sistema web para controlar o empréstimo de equipamentos compartilhados, como câmeras, notebooks, drones e projetores. Ele registra quem retirou cada item, até quando, e em que condição o item foi devolvido.

O sistema tem três tipos de usuário: o **solicitante**, que pede e devolve equipamentos; o **gestor do acervo**, que aprova pedidos e registra entregas, devoluções e manutenções; e o **administrador**, que define as regras de cada categoria e acompanha os relatórios.

## Histórias de usuário

1. Como solicitante, quero consultar os equipamentos disponíveis por categoria e período, para escolher o que posso retirar.
   - **Critério:** equipamentos emprestados, em manutenção ou fora de uso não aparecem como disponíveis.

2. Como solicitante, quero pedir o empréstimo de um equipamento informando as datas de retirada e de devolução, para garantir o uso quando eu precisar dele.
   - **Critério de recusa:** o pedido é recusado quando o equipamento já está emprestado, reservado ou em manutenção em qualquer dia do período pedido.

3. Como solicitante, quero acompanhar meus empréstimos, com os prazos de devolução, para devolver cada item no dia certo.
   - **Critério:** empréstimos com prazo vencido aparecem destacados como atrasados.

4. Como solicitante, quero cancelar um pedido que ainda não foi entregue, para liberar o equipamento para outras pessoas.
   - **Critério:** depois que o equipamento foi entregue, o pedido deixa de poder ser cancelado e só pode ser encerrado pela devolução.

5. Como gestor do acervo, quero aprovar ou negar os pedidos de empréstimo, para controlar quem leva o patrimônio.
   - **Critério de recusa:** a aprovação é recusada quando o solicitante tem algum equipamento com devolução em atraso, e a mensagem informa qual item está pendente.

6. Como gestor do acervo, quero registrar a entrega do equipamento ao solicitante, para saber quem está com cada item e desde quando.
   - **Critério de recusa:** a entrega é recusada quando o solicitante já está com o número máximo de itens emprestados ao mesmo tempo, definido para a categoria.

7. Como gestor do acervo, quero registrar a devolução informando a condição do equipamento, para que o item volte ao acervo ou siga para manutenção se estiver danificado.
   - **Critério:** um equipamento devolvido com defeito fica indisponível para novos pedidos até ser liberado.

8. Como gestor do acervo, quero enviar um equipamento para manutenção e liberá-lo quando voltar, para que ninguém pegue um item que não está em condições de uso.
   - **Critério:** o histórico do equipamento mostra cada período em que ele ficou em manutenção.

9. Como administrador, quero definir, para cada categoria, o prazo máximo de empréstimo e o limite de itens por solicitante, para adequar as regras ao valor de cada tipo de equipamento.
   - **Critério:** a alteração vale para os pedidos feitos depois dela, sem mudar os empréstimos em andamento.

10. Como administrador, quero ver um relatório dos empréstimos em atraso e dos equipamentos mais usados, para cobrar devoluções e decidir o que repor.
    - **Critério:** o relatório pode ser filtrado por categoria e por período.

## Integrantes

- Francisco Viana Maia Neto
- Murilo Maciel Rodrigues
