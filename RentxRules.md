# RENTX

## Cadastro de carro

**Requisitos funcionais**
- [ X ] Deve ser possível cadastrar um novo carro.

**Regra de negócio**
- [ X ] Não deve ser possível cadastrar um carro com uma placa já existente.
- [ X ] O carro deve ser cadastrado, por padrão, com disponibilidade.
- [ X ] O usuário responsável pelo cadastro deve ser um usuário administrador.

## Listagem de carros
**Requisitos funcionais**
- [ X ] Deve ser possível listar todos os carros disponíveis.
- [ X ] Deve ser possível listar todos os carros disponíveis pelo nome da categoria.
- [ X ] Deve ser possível listar todos os carros disponíveis pelo nome da marca.
- [ X ] Deve ser possível listar todos os carros disponíveis pelo nome do carro.

**Regra de negócio**
- [ X ] O usuário não precisa estar logado no sistema para listar.

## Cadastro de Especificação no carro
**Requisitos funcionais**
- [ X ] Deve ser possível cadastrar uma especificação para um carro.

**Regra de negócio**
- [ X ] Não deve ser possível cadastrar uma especificação para um carro não cadastrado.
- [ X ] Não deve ser possível cadastrar uma especificação já existente para o mesmo carro.
- [ X ] O usuário responsável pelo cadastro deve ser um usuário administrador.

## Cadastro de imagens do carro
**Requisitos funcionais**
- [ X ] Deve ser possível cadastrar a imagem do carro.

**Requisitos não funcionais**
- [ X ] Utilizar o multer para upload dos arquivos.

**Regra de negócio**
- [ X ] O usuário deve poder cadastrar mais de uma imagem para o mesmo carro.
- [ X ] O usuário responsável pelo cadastro deve ser um usuário administrador.
- Deve apagar a imagens que foram salvas na pasta tmp após o cadastro

## Aluguel de carro
**Requisitos funcionais**
- [ X ] Deve ser possível cadastrar um aluguel.

**Regra de negócio**
- [ X ] O aluguel deve ter duração mínima de 24 horas.
- [ X ] Não deve ser possível cadastrar um novo aluguel caso já exista um aberto para o mesmo usuário.
- [ X ] Não deve ser possível cadastrar um novo aluguel caso já exista um aberto para o mesmo carro.
- [ X ] O usuário deve estar logado na aplicação.
- [ X ] Ao realizar um aluguel, o status do carro deverá ser alterado para indisponível.

## Devolução de carro
**Requisitos funcionais**
- [ X ] Deve ser possível realizar a devolução de um carro

**Regra de negócio**
- [ X ] Se o carro for devolvido com menos de 24 horas, deverá ser cobrado diária completa.
- [ X ] Ao realizar a devolução, o carro deverá ser liberado para outro aluguel.
- [ X ] Ao realizar a devolução, o usuário deverá ser liberado para outro aluguel.
- [ X ] Ao realizar a devolução, deverá ser calculado o total do aluguel.
- [ X ] Caso o horário de devolução seja superior ao horário previsto de entrega, deverá ser cobrado multa proporcional aos dias de atraso.
- [ X ] Caso haja multa, deverá ser somado ao total do aluguel.
- [ X ] O usuário deve estar logado na aplicação.

## Listagem de Alugueis para usuário
**Requisitos funcionais**
- [ X ] Deve ser possível realizar a busca de todos os alugueis para o usuário.

**Regra de negócio**
- [ X ] O usuário deve estar logado na aplicação.

## Recuperar Senha
**Requisitos funcionais**
- [ X ] Deve ser possível o usuário recuperar a senha informando o e-mail.
- [ X ] O usuário deve receber um email com o passo a passo para a recuperação da senha
- [ X ] O usuário deve conseguir inserir uma nova senha

**Regra de negócio**
- [ X ] O usuário precisa informar uma nova senha
- [ X ] O link enviado para a recuperação deve expirar em 3 horas

## Alterar carro
**Requisitos funcionais**
- Não deve ser possível alterar a placa de um carro já cadastro.
