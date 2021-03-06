 *<h1> Fenix Tecnologia <h1>*

 *<h3>- Dieta: </h3>* Este módulo vai contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá alimentar uma lista com os tópicos de alimento, horário e quantidade.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciente deverá alimentar a mesma lista, dizendo o que ele comeu em cada refeição, as quantidades e os horários. 

 *<h3>- Alarme: </h3>* Este módulo irá contar com duas interfaces diferentes, onde a interface do profissional de nutrição irá acrescentar horário para o paciente ingerir alimentos e água.
 Na interface do paciente, irá aparecer todas as informações que foram passadas pela nutricionista ao mesmo, em contrapartida o paciênte deverá alimentar a mesma lista,confirmando os horários ou alterando conforme sua disponibilidade.
 
 *<h3>- Acompanhamento de Peso: </h3>* Módulo que ajuda o usuário a compreender seus hábitos alimentares registrando as calorias consumidas. Vai possuir monitoramento de gordura, proteínas, carboidratos e colesterol.

 *<h3>- Gráfico de Evolução: </h3>* Gráfico que ficará disponível a ambos usuários que será alimentado pelas informações que o paciente inserir no aplicativo, como taxas de colesterol e glicose, calorias ingeridas e peso  atual.

 *<h3>- Atividade Física: </h3>* Neste módulo será opcional o uso do mesmo, se o profissional de nutrição julgar necessário a realização de exercícios físicos o mesmo poderá recomendar ao seu paciente, nele terá exercícios padrões e a opção de listar um outro exercício. Na interface do paciente ele poderá conferir quais exercícios foram recomendados para ele e também um exemplo de como o exercício é executado.

 *<h3>- Agendamento de consultas: </h3>* Módulo onde o paciente pode solicitar ao seu nutricionista uma consulta não prevista.

<h2> Documento de definição de requisitos </h2>

*<h3>Requisitos Funcionais</h3>*

Requisitos Func. | Descrição | Prioridade |Depende de|
|:-----------------:|:-----------:|:------------:|:----------:|
 RF 01 |Efetuar Cadastro (Nutricionista / Paciente)| Alta|--|
 RF 02 |Efetuar Login / LogOff ( Nutricionista / Paciente )| Média|RF 01|
 RF 03 |Acessar Menu com todas as funcionalidades do app ( Nutricionista )| Média|RF 01 / RF 02|
 RF 04 |Poder criar dietas ( Nutricionista )|Alta|--|
 RF 05 |Sugerir Horários ( Alimentação, Atividade Física, Sono e etc..)| Média | RF 04 |
 RF 06 |Sugestões do Nutricionista|Baixa|--|
 RF 07 |Criação de relatórios|Alta|--|
 RF 08 |Sugestão de atividades físicas|Média|--|
 RF 09 |Exportação de dados do Excel | Alta | -- | 
 RF 10 |Agendamento de consultas|Média|--|
 RF 11 |Acessar Menu do paciente|Média|RF 03|
 RF 12 |Poder cadastrar, atualizar e excluir clientes/pacientes|Média|RF 10|
 RF 13 |Geração de relatórios|Médio|RF 10|
 RF 14 |Acompanhamento de resultados|Alto|RF 12|
 RF 15 |Primeiro acesso Paciente ( Questionário: idade , peso, altura, objetivo, sexo e exames ) | Alto | RF 02 |
 RF 16 |Atualização de cadastro ( Paciente)| Médio | RF 01 / RF 02 |
 RF 17 |Acesso ao Menu | Alto | RF 02 |
 RF 18 |Visualizar dietas e sugestão de horários estipulados pelo nutricionista (Paciente)| Alto | RF 04 / RF 05 |
 RF 19 |Questionários de acompanhamento ( Paciente ) | Médio | -- |
 RF 20 |Acompanhamento de objetivos ( Paciente ) | Médio | RF 18 | 
 RF 21 |Visualizar gráficos de evolução ( Paciente ) | Médio | RF 18 / RF 19 |
 RF 22 |Visualizar sugestões de atividades físicas ( Paciente )| Médio | RF 08 | 
 RF 23 | Agendamento e cancelamento de consultas | Baixo | -- |



*<h3>Regras de Negócio</h3>*

Regras de Negócios| Descrição |Prioridade| Depende de.|
|:----------:|:-----------:|:------------:|:----------:|
 RN 01|Para se cadastrar o nutricionista deve inserir um CRN válido|Alta|RF 01|
 RN 02|O sistema deve contar com um sistema ant-robô ( Captcha )|Alta|--|
 RN 03|O sistema deve aceitar cadastro via e-mail ou redes sociais para o paciente|Alta|--|
 RN 04|As informações guardadas em bancos de dados devem ser encriptadas|Alta|--|
 RN 05|As informações alteradas pelos usuários devem ser atualizadas no aplicativo em até 30 segundos|Média|--|
 RN 06|O sistema deve suportar informações sendo alteradas pelo Nutricionista e pelo paciente simultâneamente|Alta|--|
 RN 07|O sistema deve contar com interface Mobile e futuramente interface web ( Rodar em diferentes sistemas Mobile como Android e IOS e futuramente colocaremos nossa interface na web rodando em Navegadores.)|Alta|--|
 RN 08|Os dados coletados através do preenchimento dos questionarios serão utilizadas na criação dos gráficos de acompanhamento| Baixa | RF 18 |
 RN 09|Deverá existir a função de excluir todas as informações de usuário do sistema|Alta|--|
 RN 10|Gráficos devem ser atualizados semanalmente| Média | RF 08|
 RN 11|Senhas de usuários deverão contar com caracteres, numerais e símbolos, totalizando pelo menos 8 dígitos na senha|Alta|--|
 RN 12|O sistema deve ser capaz de diferenciar no ato acesso, se é o nutricionista ou o paciente quem está logando. | Alta | RF 02|
 RN 13|O sistema após o login deve atualizar em até 3 segundos| Alto | -- |
 RN 14|O nutricionista deve ser capaz de exportar dados de seus pacientes no formato de arquivo excel | Alta | 02 | 

*<h3>Requisitos não funcionais</h3>*
Requisitos Não F. | Descrição |  Categoria |  Escopo  |Prioridade| Depende de. |
:-----------------: |:-----------:|:------------:|:----------:|:----------:|:------------:|
 RNF 01|As Informações cadastradas deverão ser guardadas em um banco dados protegido por criptografia|Segurança de acesso|Sistema|Alta|RN 01|
  RNF 02|O sistema deve oferecer a opção de leitura, alteração e exclusão de informações cadastradas|Segurança de dados|Funcionalidade|Alta|RF 03|
 RNF 03|Sistema deve apresentar um questionário inicial contendo algumas informações no primeiro acesso|Usabilidade|Sistema|Média|RF 04|
RNF 04|O Sistema deve conter funcionalidades diferentes nas interfaces do profissional e do  paciente.|Interoperabilidade|Sistema|Alta|--|
 RNF 05|O sistema deverá contar com gráficos e dashboard para os usuários acompanharem sua evolução|Usabilidade|Sistema|Média|RF 09|
 RNF 06|O sistema deverá ter um menu com recomendações de exercícios físicos que possam corroborar com as dietas estipuladas|Usabilidade|Funcionalidade|Baixa|--|
 RNF 07|O sistema vai contar com a opção de marcar consultas online ou presenciais fora de agenda.|Atratividade|Funcionalidade|Média|--|
 RNF 08 |O sistema deve permitir aos usuários estarem efetuando LogOff do sistema perdendo assim todos os acessos às informações confidenciais.|Segurança de informação|Sistema|Alta| -- |
 RNF 09 | O usuário deverá ser capaz de alterar seus objetivos dentro do aplicativo | Usabilidade | Funcionalidade | Média | -- |   
