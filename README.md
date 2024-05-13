# learning-irpf
Neste contexto IRPF (**I**mposto sobre a **R**enda das **P**essoas **F**ísicas) vai estar se referindo ao software que o governo criou para podermos informalos do nosso imposto de renda.  

Download: https://www.gov.br/receitafederal/pt-br/centrais-de-conteudo/download/pgd/dirpf  

Todo ano se deve baixar a versão daquele ano para fazer o imposto de renda do ano passado.  
Em outras palavras, você baixa o IRPF de 2024 para fazer o imposto de renda de 2023.   

# Start
Todo imposto de renda envolve você dizer os valores no ano X ao mesmo tempo que mostra o IRPF mostra como eles estavam em X-1.  

Por exemplo, para IRPF 2024:
| 2022   | 2023   |
| ------ | ------ |
| R$50,0 | R$75,0 |

Entendeu? Estou utilizando o IRPF de **2024** para preencher sobre o ano de **2023** e enquanto o programa mostra como estava em **2022**.  

## Start import
IRPF vai dar 3 opções de criação da declaração:
- Iniciar Declaração em Branco
  - Se é a sua primeira declaração da vida, é essa opção que você deve selecionar
- Iniciar Importando Declaração de XXXX
  - Caso você tenha feito backup, você pode importar informações do IPRF passado com essa opção
- Iniciar Declaração a partir da Pré-Preenchida
  - Caso sua conta do governo (gov.br) seja eligível, você pode ter seu IRPF pré pronto
  - A recomendação é sempre validar se nada foi preenchido incorretamente (sim, isso já aconteceu antes)

# Backup
O sistema oferece armazenar na núvem deles mas a recomendação é sempre fazer o backup manual também.  

Já aconteceu de sistemas do governos sofrerem com [ransomware](https://en.wikipedia.org/wiki/Ransomware) (malware que bloqueia acesso a dados até que se pague os hackers), então é recomendado que você tenha o backup na sua núvem de preferência (icloud/google drive/onedrive).  

## Backup formats
Existem 3 formatos de arquivos únicos do IRPF:  
- `.DBK`
  - Backup do estado dos dados preenchidos até o momento
    - Esse backup é usado para caso você queira parar de editar a declaração no meio e queira voltar a editar ela mais tarde
- `.REC`
  - Backup da **Rec**eita
    - Esse backup deve ser importado no início da declaração do ano seguinte
      - Ao menos que isso seja feito automaticamente pelo IRPF
      - Não se precisa fazer isso se nunca fez imposto de renda antes
  - Nome do arquivo: `{0}-IRPF-A-{1}-{2}-ORIGI.REC`
    - `{0}`: Os números do seu CPF
    - `{1}`: Ano feito
    - `{2}`: Ano do qual se refere
    - Exemplo: `12345678901-IRPF-A-2024-2023-ORIGI.REC`
  - **Observação**: `.rec` também é um formato de video então se você tiver um video player, ele talvez ache que é um video e bote o ícone do video player 😆
    - Isso não é um problema! Só ignore e siga sua vida.
- `.DEC`
  - Backup da **Dec**laração
    - Esse backup deve ser importado no início da declaração do ano seguinte
      - Ao menos que isso seja feito automaticamente pelo IRPF
      - Não se precisa fazer isso se nunca fez imposto de renda antes
  - Nome do arquivo: `{0}-IRPF-A-{1}-{2}-ORIGI.DEC`
    - `{0}`: Os números do seu CPF
    - `{1}`: Ano feito
    - `{2}`: Ano do qual se refere
    - Exemplo: `12345678901-IRPF-A-2024-2023-ORIGI.DEC`
  - Este arquivo armazena justamente suas declarações, ou seja, qualquer coisa que você tenha "preenchido" durante o IRPF
    - Hoje em dia tem o preenchimento automático para muitas informações. Por exemplo: dados vindo do banco
      - Porém caso tenha sido uma compra de pessoa física ou venda para pessoa física, você ainda deve ter que preencher manualmente

## Backup files
Ao final do IRPF o botão "Gravar Cópia" vai ficar disponível para apertar.  

Use ele para criar os backups (`.REC`, `.DEC`) e criar um recibo (`.pdf`) dizendo que você declarou, salve tudo na sua núvem pessoal e aceite salvar na núvem do governo.  
