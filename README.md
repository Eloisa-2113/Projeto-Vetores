O que é o Vector?
Definição: É uma classe do Java (pertencente ao pacote java.util) que implementa uma estrutura de dados de array dinâmico.
Objetivo: Foi criado para resolver a limitação dos arrays tradicionais, cujo tamanho é fixo e não pode ser alterado após a criação. O Vetor cresce ou diminui de tamanho automaticamente conforme você adiciona ou remove elementos.
Como ele funciona por dentro? Capacidade Inicial: Quando você cria um Vector, ele reserva um espaço inicial na memória (geralmente para 10 elementos, se não for especificado).Redimensionamento: Quando o Vector fica cheio e você tenta adicionar mais um elemento, ele cria um novo array interno com o dobro do tamanho do anterior e copia todos os dados antigos para esse novo espaço.
Principais Características TécnicasIndexado: Cada elemento possui uma posição numérica (índice) que começa em $0$. O acesso a um elemento via índice é extremamente rápido.
Sincronizado (Thread-Safe): Todos os métodos principais do Vector utilizam a palavra-chave synchronized. Isso significa que se duas ou mais threads tentarem alterar o Vector ao mesmo tempo, o Java garante que elas não vão corromper os dados (uma espera a outra terminar).
Permite Duplicatas e Nulos: Você pode salvar elementos repetidos e também o valor null.
Mantém a Ordem: Os elementos ficam exatamente na ordem em que foram inseridos.
