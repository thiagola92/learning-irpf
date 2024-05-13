# learning-irpf
Neste contexto IRPF (**I**mposto sobre a **R**enda das **P**essoas **F**ísicas) vai estar se referindo ao software que o governo criou para podermos informalos do nosso imposto de renda.  

Download: https://www.gov.br/receitafederal/pt-br/centrais-de-conteudo/download/pgd/dirpf  
Todo ano se deve baixar a versão daquele ano.  

# Backup
O sistema oferece armazenar na núvem deles mas a recomendação é sempre fazer o backup manual também.  

Já aconteceu de sistemas do governos sofrerem com [ransomware](https://en.wikipedia.org/wiki/Ransomware) (malware que bloqueia acesso a dados até que se pague os hackers), então é recomendado que você tenha o backup na sua núvem de preferência (icloud/google drive/onedrive).  

## Backup formats
Existem 3 tipos de arquivos únicos do IRPF:  
- `.DBK`
  - Backup do estado dos dados preenchidos até o momento
    - Esse backup é usado para caso você queira parar de editar a declaração no meio e queira voltar a editar ela mais tarde
- `.REC`
  - Backup da **Rec**eita
    - Esse backup deve ser importado no início da declaração do ano seguinte
      - Ao menos que isso seja feito automaticamente pelo IRPF
  - Nome do arquivo: `{0}-IRPF-A-{1}-{2}-ORIGI.REC`
    - `{0}`: Os números do seu CPF
    - `{1}`: Ano feito
    - `{2}`: Ano do qual se refere
    - Exemplo: `12345678901-IRPF-A-2021-2020-ORIGI.REC`
  - **Observação**: `.rec` também é um formato de video então se você tiver um video player, ele talvez ache que é um video e bote o ícone do video player 😆
    - Isso não é um problema! Só ignore e siga sua vida.
- `.DEC`
  - Backup da **Dec**laração
    - Esse backup deve ser importado no início da declaração do ano seguinte
      - Ao menos que isso seja feito automaticamente pelo IRPF
  - Nome do arquivo: `{0}-IRPF-A-{1}-{2}-ORIGI.DEC`
    - `{0}`: Os números do seu CPF
    - `{1}`: Ano feito
    - `{2}`: Ano do qual se refere
    - Exemplo: `12345678901-IRPF-A-2021-2020-ORIGI.DEC`
  - Este arquivo armazena justamente suas declarações, ou seja, qualquer coisa que você tenha "preenchido" durante o IRPF
    - Hoje em dia tem o preenchimento automático para muitas informações. Por exemplo: dados vindo do banco
      - Porém caso tenha sido uma compra de pessoa física ou venda para pessoa física, você ainda deve ter que preencher manualmente

## Backup files
Ao final do IRPF, é recomendado que você tenha baixado os arquivos do formato `.REC` e `.DEC` e feito backup deles na sua núvem.  

Além destes dois arquivos com o formato único do IRPF, também é recomendado que você tenha baixado o arquivo `.pdf` com o resumo do ocorrido.  
