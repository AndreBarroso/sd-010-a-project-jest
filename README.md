# Boas vindas ao repositório do projeto Jest Assíncrono e Mocking!
Este projeto, teve como objetivo implementar testes utilizando o **Jest** para verificar se uma série de funções funcionavam corretamente. Foi colocado em prática o conteúdo que aprendido sobre Jest assíncrono e Mocks aplicados a testes em Javascript. 

Os principais desafios e aprendizados que tirei desse projeto foi em relação à mocagem de funções. Esse foi um conteúdo que a principio achei bastante abstrato mas que durante a execução do projeto pude entender bem qual a sua motivação. Vejamos, se eu utilizo em minha aplicação um conteúdo de terceiros como uma API, o que fazer se houver a necessidade de testar minha aplicação mas naquele momento o conteúdo externo está fora do ar? É aí que entra a mocagem que tem a função de simular a requisção da API, na execução do teste.

---

## Habilidades

- Escrever testes para funções assíncronas;
- Aplicar os seus conhecimentos acerca de testes utilizando o Jest;
- "Mockar" funções;
- "Mockar" APIs;

---

## Instruções para executar o projeto em seu próprio computador


1. Abra o terminal, acesse o diretório de sua preferência onde 
você deseja fazer o download, e crie uma pasta usando o comando **mkdir**:
```bash
mkdir projeto-andre
```

2. Entre no diretório que você acabou de criar: 
```bash
cd projeto-andre
```

3. Faça o clone do projeto executando o comando a seguir:
```bash
git clone https://github.com/AndreBarroso/sd-010-a-project-jest.git
```
4. Acesse a pasta criada executando o comando a seguir:
```bash
cd sd-010-a-project-jest
```

5. Instale as dependências do projeto executando:
```bash
npm install;
```

6. Para rodar os testes, execute o comando abaixo:
```bash
npm test;
```
Para quaisquer dúvidas, entre em contato comigo pelo email: andrefb.eng1@gmail.com .

---

### Lista de requisitos

### 1 - Crie testes para uma função assíncrona

Complete os testes do arquivo `test/asyncJest.spec.js` para que funcionem com código assíncrono.

### 2 - Crie um "Mock" no arquivo test/mockFunctions.spec.js

Crie mock functions no arquivo `test/mockFunctions.spec.js` para que os testes mockados 'sobrescrevam' o código definido na pasta `src`. A idéia é que as funções criadas a partir do Jest tenham prioridade na sua execução.

### 3 - Crie um Mock para o retorno da API

Crie uma API mock no arquivo `test/mockApi.spec.js` para que os testes do Jest utilizem retornos de API fixos e independentes de requisições.

Exemplo de resposta da API randomuser.me:

```js

{
  gender: 'female',
  name: { title: 'Ms', first: 'Deborah', last: 'Hanson' },
  location: {
    street: { number: 1299, name: 'Rochestown Road' },
    city: 'Birr',
    state: 'Wicklow',
    country: 'Ireland',
    postcode: 16223,
    coordinates: { latitude: '26.2451', longitude: '45.2995' },
    timezone: {
      offset: '+5:30',
      description: 'Bombay, Calcutta, Madras, New Delhi'
    }
  },
  email: 'deborah.hanson@example.com',
  login: {
    uuid: '45db2b1f-1c9a-4a80-9572-e46614f86c30',
    username: 'bluewolf366',
    password: 'iverson3',
    salt: 'XKOOGc2x',
    md5: '8cb7b4686f3869247b3ed189de780ea6',
    sha1: 'c24641f415cf36f4494ea4007fb3d77b47a6aad5',
    sha256: 'a7bdd079ead0adf21f30cee5b94e5581a9fa0d5fc8b3c1881dbc864dabc55a80'
  },
  dob: { date: '1965-10-01T06:35:49.694Z', age: 55 },
  registered: { date: '2009-02-11T05:48:39.772Z', age: 11 },
  phone: '021-953-7205',
  cell: '081-160-6277',
  id: { name: 'PPS', value: '0109675T' },
  picture: {
    large: 'https://randomuser.me/api/portraits/women/7.jpg',
    medium: 'https://randomuser.me/api/portraits/med/women/7.jpg',
    thumbnail: 'https://randomuser.me/api/portraits/thumb/women/7.jpg'
  },
  nat: 'IE'
}

```

### 4 - Crie funções no arquivo test/setupTeardown.spec.js

Intercale funções entre os testes definidos no arquivo `test/setupTeardown.spec.js`.

---
