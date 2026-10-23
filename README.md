# OpenWeb



O OpenWeb é um navegador de código aberto para Windows x64. Usa Electron e Chromium, com a interface em HTML, CSS e JavaScript. O código-fonte está disponível para leitura, cópia e modificação sob a licença MIT; veja `LICENSE` e **Compilar a partir do código-fonte**.

> O OpenWeb não é escrito inteiramente em C. A interface do navegador usa HTML, CSS e JavaScript dentro do Electron; o mecanismo de páginas é o Chromium, que inclui componentes nativos em C/C++.

## Recursos

- Abas, barra de endereço e pesquisa, voltar, avançar e recarregar.
- Ícone de cada site exibido ao lado do nome da aba.
- Menu de abas e acesso direto a Downloads, perfil e opções do navegador.
- Bloqueador de anúncios opcional, ativado por padrão, com filtros públicos da comunidade.
- Modo **Alto desempenho**, que mantém abas em segundo plano ativas, e modo **Equilibrado**, que reduz a atividade dessas abas.
- Aceleração gráfica do Chromium quando disponível. A mudança dessa opção requer reiniciar o OpenWeb.
- WebGL e WebAssembly para páginas e jogos compatíveis com o Chromium e com o computador.
- Pasta de downloads configurável e opção para escolher o destino antes de cada download.
- Lista de atividade com downloads e histórico. Nomes de arquivos repetidos recebem um sufixo para evitar sobrescrever um arquivo existente.
- O progresso animado dos downloads também aparece enquanto as configurações estão abertas.
- A lista de downloads mostra o ícone do site, tamanho em MB/GB, velocidade em MB/s e Mbps, porcentagem e botão para cancelar arquivos em andamento.
- Restaura as abas abertas ao reiniciar. Configurações, histórico, cookies e downloads do usuário permanecem salvos durante atualizações.
- Clique com o botão direito em uma imagem para salvá-la diretamente em Downloads; **Inspecionar elemento** abre as ferramentas de desenvolvimento.
- Tema claro ou escuro, página inicial e mecanismo de pesquisa configuráveis.
- Atalho para as configurações do Windows ao definir o OpenWeb como navegador padrão.

## Requisitos do computador

### Necessários

- Windows 10 ou posterior, 64 bits.
- Processador x64.
- 4 GB de memória RAM para navegação básica.
- Conexão com a internet para abrir sites. O bloqueador precisa buscar filtros públicos na primeira inicialização, quando não há cache local.
- Cerca de 500 MB de espaço livre para instalar o navegador e seus componentes.

### Recomendados

- 8 GB de memória RAM para várias abas, jogos e páginas pesadas.
- Driver de vídeo atualizado e compatível com aceleração gráfica/WebGL para melhor desempenho em conteúdo 3D.
- SSD e conexão estável para uma experiência mais responsiva. A velocidade dos downloads depende também da rede e do servidor do site.

O instalador publicado nesta versão é para Windows x64. Electron 44 exige Windows 10 ou posterior e oferece binários de 64 bits; veja a [política de plataformas do Electron](https://www.electronjs.org/docs/latest/breaking-changes).

## Instalação no Windows

Baixe `OpenWeb-1.4.8-x64.exe` na seção **Releases** do GitHub e execute o instalador. Se já houver uma instalação do OpenWeb com o mesmo identificador, o instalador pode atualizar os arquivos no mesmo destino. O perfil e as preferências do usuário ficam guardados durante a atualização. O arquivo `OpenWeb-1.4.8-source.zip` contém os arquivos usados para compilar e modificar o projeto.

O instalador não tem assinatura digital. O Windows pode exibir um aviso ao baixar ou iniciar o arquivo. Publicar futuras atualizações requer gerar uma nova versão e anexar o novo instalador a uma release. O navegador ainda não tem um serviço de atualização automática configurado.

## Downloads

O OpenWeb usa o sistema de rede de downloads do Chromium. É possível escolher uma pasta padrão ou pedir ao navegador o local de cada arquivo. A seção Downloads mostra os itens em andamento, concluídos ou interrompidos. A retomada de uma transferência interrompida depende do site e do suporte do servidor; a velocidade depende da conexão, do computador e do servidor remoto.

## Compilar a partir do código-fonte

1. Instale Node.js 22.12 ou posterior.
2. Abra a pasta `OpenWeb` em um terminal.
3. Execute `npm install` para instalar as dependências.
4. Execute `npm start` para abrir o navegador em desenvolvimento.
5. Execute `npm run dist` para criar o instalador NSIS em `dist/`.

## Privacidade

O histórico e as preferências do navegador são armazenados no perfil local do usuário. O OpenWeb não inclui uma conta ou sincronização na nuvem. Sites visitados recebem conexões normais do navegador; o bloqueador de anúncios busca e armazena localmente os filtros públicos necessários.

## Tecnologias e licença

- Electron 44 e Chromium distribuído com o Electron.
- Interface em HTML, CSS e JavaScript.
- Ghostery Adblocker para filtrar anúncios (MPL-2.0).
- O código do OpenWeb está sob a licença MIT, disponível em [`LICENSE`](LICENSE). As dependências mantêm suas próprias licenças.

## Versão

Versão atual: **1.4.8** (Windows x64).
