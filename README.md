# FLOWPODCAST

Fala meus nobres flowers, muito obrigado pelo interesse em participar da iniciativa Open Source do nosso Fórum.

Estamos dando um passo muito importante em nossa comunidade, buscando a galera criativa para mexer com o nosso querido fórum. Abri essa discussão no canal de inovação onde poderemos ter um canal aberto e transparente, um local onde está 100% liberado o brainstorm coletivo, por isso, nenhuma ideia é merda, solta o que tu pensa e vamos lapidar juntos!

Trago aqui algumas das sugestões que eu tenho e algumas que estamos pensando em conjunto internamente, e adoraria ouvir feedbacks e novas sugestões!



# IDEIAS FÓRUM FLOW PODCAST

* criação de tópicos
* cada tópico seria como se fosse uma thread, então há a possibilidade de responder o tópico e responder as respostas do tópico e assim por diante
* cada tópico e reply possuirá sistema de upvote e downvote, fazendo com que o algoritmo priorize e dispare no feed do usuário apenas aquilo que é relevante pra comunidade em si e despriorize o que recebe muito downvote
* cada tópico poderá ser criado com texto, imagem, vídeo, emojis e formatação markdown ou HTML
* configuração do perfil do usuário
* sistema de grupos, cada grupo haverá N tópicos
* sistema de gerenciamento de grupos, cada usuário poderá criar quantos grupos quiser e quantos tópicos quiser
* invite de usuários para gerenciamento de grupos
* sistema de emblemas pra gerar gamificação de acordo com a atividade do usuário na plataforma
* me conta aí, o que vc acha que podemos implementar?



# INFORMAÇÕES PARA NOVOS DESENVOLVEDORES

Lembrando que a loja, plataforma de apoio e fórum são 3 pilares independentes, estou usando React JS na versão 1.0 da loja, apenas pelo motivo que tenho mais facilidade com react js, mas não que eu queira que ele seja focado nessa stack, acho que o consenso de geral deverá prevalecer em relação ao porte que o fórum pretende ser.

Estou vendo em questão de infra / custos pra disponibilizar um sistema de criação de chaves de API, além disso, preciso mapear quais serão as APIs que poderão ser disponibilizadas.
A ideia é de que qualquer desenvolvedor possa solicitar uma chave de API e começar a montar algo relativo ao fórum / flow, utilizando informações que a equipe oficial do flow provê

A loja e plataforma de apoio são frentes separadas desse tópico aqui (aqui nessa organização o foco é o fórum), lembrando também que apenas o fórum é open source e colaborativo, até esse momento.



# API de Login de Usuários | Cadastro Unificado

Nossa base atualmente está com os seguintes dados, pensando em uma loja virtual

* authorize: bool => política de privacidade
* city: string => cidade do usuário
* company_name: string caso type_document === cnpj => nome da empresa
* complement: string => complemento do endereço do usuário
* country: string => país do usuário
* created_at: timestamp => data de registro do usuário
* document: string => cnpj ou cpf formatado
* first_name: string => primeiro nome do usuario
* last_name: string => ultimo nome do usuário
* level_access: int => nível de acesso do usuário | 0 = usuário | 1 = vip | 2 = mod | 3 = admin
* neighborhood: string => bairro do usuário
* phone: string => telefone formatado
* sex: string => sexo do usuário
* state: string => estado do usuário
* state_registration: string => inscrição estadual caso type_document === cnpj
* status_account: bool => status da conta do usuário
* street: string => nome da rua do usuário
* type_document: string => cpf ou cnpj
* updated_at: timestamp => ultima vez q perfil do usuário foi alterado
* zipcode: string => cep do usuário

Como vocês podem aproveitar essas informações para que a modelagem do fórum se inicie?
Como posso ajudar nessa questão também? Lembrando que temos a LGPD para respeitar.

A ideia é que eu possa criar uma API que vocês possam consumir, pensei em algo do tipo Login através do Flow, assim como no facebook

assim vocês podem se sentir à vontade para startar qualquer projeto, utilizando a mesma base de dados do flow para usuários, assim podemos integrar em um futuro próximo com ações do fórum, por exemplo subir de rank do usuário.

pensando em integrações futuras com o fórum, vejo esse caminho de login unificado super interessante, mas não é algo que necessitamos por agora.

Outro ponto é que pensando em algo como o facebook faz, para cada aplicativo utilizar informações do Flow, terá de passar por uma aprovação, a fim de verificarmos quais as intenções do seu aplicativo, como você utilizará tal integração, para que possamos criar um ambiente seguro para todos os flowers e também não se fudermos em questão de LGPD, cambridge analytics tá aí pra provar que dá pra tomar muito no cu em questões monetárias, então fiquem espertos por favor



