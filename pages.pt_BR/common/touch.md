# touch

> Cria arquivos e define tempo de acesso/modificação.
> Mais informações: <https://manned.org/touch>.

- Cria arquivos especificados:

`touch {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Define o tempo de [a]cesso ou [m]odificação do arquivo como o atual e não [c]ria o arquivo se ele não existir:

`touch {{[-c|--no-create]}} -{{a|m}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Define o [t]empo do arquivo para um valor especificado e não [c]ria o arquivo se ele não existir:

`touch {{[-c|--no-create]}} -t {{YYYYMMDDHHMM.SS}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Define o tempo de um arquivo específico para o tempo de out[r]o arquivo e não [c]ria o arquivo se ele não existir:

`touch {{[-c|--no-create]}} {{[-r|--reference]}} {{~/.emacs}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`
