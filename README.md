
# WhatsAp2p
Computer Engineering class taken in 2020/1

##### Objetivo: Obter conhecimentos básicos para o desenvolvimento de software peer-to-peer (P2P) em ambientes TCP/IP. Implementar um sistema de envio de mensagens de texto e foto peer-to-peer (WhatsAp2p) em linguagem C.

### Módulos
#### -  Servidor central
> O **servidor central** deverá permitir aos usuários localizar os demais usuários online. Cada usuário é identificado no servidor central por um **número de telefone** e sua localização corresponde ao **endereço IP** e à porta onde o módulo de usuário deste usuário aguardará por mensagens e fotos.
> 
#### - Módulo de usuário
> O **módulo de usuário** deverá permitir ao usuário enviar mensagens e fotos a outros usuários e também receber mensagens e fotos de outros usuários, a partir das informações de localização obtidas do **servidor central**.

## Requisitos do Projeto

O **módulo de usuário** inicia a conexão informando ao **servidor central**: um **número de telefone**, **IP** e **porta** em que aguardará por conexões para a troca de mensagens P2P.

O **servidor central** armazena então os dados de identificação registrando este usuário como online (chat disponível). Usuários não registrados no **servidor central** são identificados como **offline** (chat indisponível) e por consequência incapazes de receber mensagens e ou fotos.

O usuário deve ser capaz de adicionar um **contato e também criar grupos de contatos**, tais informações são armazenadas em um **arquivo local** e também pré carregadas na inicialização.

Ao solicitar cada envio de mensagem (texto ou foto) a um contato ou a um grupo, o **módulo de usuário** deve realizar uma **consulta ao servidor central** para obter a **disponibilidade** desse(s) contato(s) e, em seguida o conteúdo da **mensagem** deve ser enviado diretamente à localização do contato, sem passar pelo servidor central (P2P).

Quando um usuário finalizar o seu **módulo de usuário**, toda informação relativa à localização deste usuário deve ser removida do **servidor central** (o usuário fica indisponível na central). 

- O **servidor central** e os **módulos de usuário** devem suportar acesso concorrente.
- Deve ser possível executar mais de um **módulo de usuário** no mesmo computador.
- O endereço de IP e a porta do servidor central deverão ser passados como parâmetro para o **módulo de usuário** na linha de comando.

## Ambiente de Desenvolvimento

## Processo de Compilação

##  Demonstrações
