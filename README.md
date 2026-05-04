## ANOTAÇÕES IMPORTANTES

`Staging: ` Área de preparação.
Você o utiliza para informar ao Git exatamente quais 
arquivos deseja incluir no seu próximo commit.
Isso lhe dá controle sobre o que entra no histórico do seu projeto.

`Commit do git:`o Commit é o conceito mais importante do Git. Se fôssemos explicar para uma criança de 5 anos, seria assim:

Imagine que você está jogando um videogame muito difícil. Você acabou de passar de uma fase complicada e não quer perder seu progresso se morrer na próxima fase. O que você faz? Você salva o jogo.

Melhores práticas para mensagens de compromisso:
Mantenha a primeira linha curta (50 caracteres ou menos).
Use o modo imperativo (ex.: "Adicionar recurso" e não "Recurso adicionado").
Deixe uma linha em branco após o resumo e, em seguida, adicione mais detalhes, se necessário.
Descreva por que a mudança foi feita, e não apenas o que mudou.

o Commit é o conceito mais importante do Git. Se fôssemos explicar para uma criança de 5 anos, seria assim:

Imagine que você está jogando um videogame muito difícil. Você acabou de passar de uma fase complicada e não quer perder seu progresso se morrer na próxima fase. O que você faz? Você salva o jogo.

O Commit não é apenas uma cópia de segurança; ele é uma fotografia (snapshot) do seu projeto naquele exato momento.

A Mudança: Você escreve um código ou altera um arquivo.

A Preparação (Staging): Você diz ao Git: "Olha, eu quero salvar estas alterações aqui".

O Commit: Você bate a foto. O Git registra quem fez, quando fez e o que foi mudado.

Muitos desenvolvedores tratam o commit como uma "obrigação de fim de dia". Eles trabalham 8 horas e fazem um único commit chamado "ajustes". Isso é um erro grave.

O Erro: Fazer commits gigantes (monolíticos). Se algo der errado, você terá que desfazer 8 horas de trabalho.

A Oportunidade: Commits devem ser atômicos. Fez uma pequena função que funciona? Commit. Corrigiu um erro de digitação? Commit.

A Verdade: O commit é a sua máquina do tempo. Se você não salvar em pequenos intervalos, sua máquina do tempo terá poucas paradas e você ficará "preso" no presente se o código quebrar.

Para ser um profissional respeitado, seu commit precisa de duas coisas:

O Conteúdo: As alterações reais no código.

A Mensagem: Um texto curto explicando o porquê daquela mudança (e não o "o quê").

Exemplo ruim: git commit -m "mudei o código"
Exemplo profissional: git commit -m "Corrige o cálculo do imposto para rendimentos acima de 5k"

`git commit -a -m` "message"

Este é o comando para os "preguiçosos" (ou práticos). Imagine que você está com pressa e quer salvar o jogo agora, sem precisar conferir o que está na bolsa.

O que ele faz: O -a vem de all (tudo). Ele pula a etapa de você ter que dizer "adicione este arquivo" (git add). Ele pega todos os arquivos que o Git já conhece e que foram modificados e faz o save de uma vez.

O Perigo: Ele não salva arquivos novos que você acabou de criar (arquivos untracked). Se você criou um arquivo novo chamado Calculadora.java e rodar esse comando, ele ficará de fora.

Dica Profissional: Use este comando apenas quando você tem certeza absoluta de que tudo o que mudou deve ser salvo. Caso contrário, você acabará enviando "lixo" ou código incompleto para o histórico.

`Palavra chave antes de pensar em dar um commit: ` Se eu aplicar esse commit, 
ele vai...

`Mais dicas para dar um commit:`

Um commit bem estruturado deve responder a três perguntas no seu corpo:

Por que esta mudança é necessária?

Como ela resolve o problema?

Quais são os efeitos colaterais ou quebras de compatibilidade?