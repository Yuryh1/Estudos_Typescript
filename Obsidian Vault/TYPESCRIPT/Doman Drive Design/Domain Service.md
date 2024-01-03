Realiza tarefas específicas do domínio, não tendo estado. É indicado quando a operação que você quer executar não pertence a uma entity ou a um value object Exemplos DistanceCalculator: Pegando duas coordenadas retorna a distância FareCalculator: Calcula o valor de um segmento da corrida TokenGenerator: Gera um token de acordo com um email


Utilize em operações que envolvem múltiplos objetos de domínio Normalmente quando uma operação afeta múltiplos objetos de domínio, não pertencendo a nenhum deles, ela deve ser descrita em um domain service