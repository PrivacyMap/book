### Rastreamento digital

##### No mundo em que vivemos, é imposssível obter privacidade e anonimato absolutos, sendo recomendado a criação de múltiplas identidades e a posterior alocação compartimentalizada.

##### Abaixo, serão apresentadas as principais formas de rastreamento no mundo digital, não sendo, portanto, uma revisão integrativa sobre o tema.

##### As técnicas de rastreamento estão avançando nos últimos anos. Novas tecnologias, como o  HTML5, possibilitaram novas maneiras de obtenção de dados dos usuários.
Vamos iniciar com uma tecnologia mais antiga, com menor relevância nos rastreamentos mais sofisticados, mas que merece nossa atenção: cookies.

##### Cookies são pequenos arquivos em seu computador que armazenam informações relevantes para a sua navegação. Alguns cookies são úteis para o usuário, como aqueles
que guardam as preferências dos sites que visitamos com frequência ou os que guardam dados dos produtos em nosso carrinho, quando efetuamos alguma compra online.
Não precisamos adicionar os produtos novamente, pois as informações de nossa sessão estão armazenadas no cookie.

##### Alguns cookies, por outro lado, são utilizados para rastrear os hábitos de navegação do usuário para propósitos comerciais. Por si só, nada de errado. O problema
surge por causa:

##### *da falta de transparência do processo, com a maioria dos usuários desconhecendo as práticas adotadas;

##### *da quantidade de informações coletadas, podendo ser suficientes para traçar um perfil completo dos interesses do usuário;

##### *do armazenamento das informações coletadas por tempo desconhecido, por vezes, indeterminado;

##### *do compartilhamento das informações coletadas com terceiros dos mais diversos, nem sempre bem intencionados.  

##### Podemos dividir os cookies em:

#### First-party cookies (mesma origem)

##### Podem ser persistentes ou efêmeros. Apresentam menor preocupação quanto à privacidade, mas podem ser utilizados para rastreio e construção de perfil.
Utilizados apenas pelo site de origem.

#### Third-party cookies (de terceiros)

##### Podem ser persistentes ou efêmeros. Acessados por sites que não os criaram, aumentando a capacidade de rastreamento frente aos de mesma origem. A
transmissão das informações armazenadas no cookie não necessita de interação do usuário, bastando o site, com conteúdo de anunciantes e/ou de redes sociais,
ser carregado.

### Endereços IP 

##### Os endereços IP (internet protocol) são os mais utilizados para o rastreamento na internet. Por meio dessa informação, pode(m) ser:

##### revelada a localização física aproximada;

##### auxiliada a identificação de dispositivos de hardware utilizados na navegação, como modems ou celulares;

##### reveladas as atividades peer-to-peer (P2P) vinculadas ao endereço em questão;

##### rastreados fragmentos em servidores web diversos, possivelmente construindo um perfil de navegação e identificação.

##### Pode-se utilizar um serviço de VPN confiável como: Mullvad VPN, IVPN e ProtonVPN, ou a rede Tor.

### Geolocalização

##### Sua localização, para a privacidade, é uma das informações mais importantes disponíveis. Nos navegadores mais comuns, o pedido de permissão geralmente
aparece em uma caixa de texto, no canto superior da tela, quando o navegador acessa um site que solicita saber sua localização. 

##### Adicionalmente à criação de uma mapa 3D das ruas e cidades, projetos como o Google Street View tinham propósitos pouco conhecidos pelo público em geral.
Um deles era o mapeamento, a nível global, das redes wifi. Por meio desse mapa global que associa localização com determinada rede, os browsers atuais têm a
capacidade de saber a localização do usuário por meio da triangulação das redes próximas associadas ao seu endereço de ip. Usos para essa tecnologia incluem a
praticidade da detecção de serviços próximos, como pizzarias ou outros estabelecimentos com delivery, porém, essa informação pode ser utilizada para compor perfis
detalhados em bases de dados diversas. Se habilitado pelo usuário, a precisão desse método pode chegar a dois metros.

### Rastreio por identificadores em URLs

##### Anunciantes e empresas utilizam parâmetros nos endereços web para a coleta de informações acerca do grau de sucesso de seus anúncios. Adicionalemnte, esse
tipo de rastreamento pode ocorrer quando um website adiciona identificadores únicos às URLs antes do usuário deixar o site. Scripts nos sites de destino podem,
então, ler o identificador, obtendo conhecimento sobre parte da navegação do usuário. 

### Mouse fingerprinting e padrões de digitação

##### O rastreamento do cursor do mouse ocorre com a coleta de dados por meio de softwares. O rastreio pode acontece com o uso de JavaScript, CSS, plugins ou
softwares específicos. Essa tecnologia de rastreio proporciona a coleta:

*da localização do ponteiro
*dos cliques efetuados
*do tempo em que se permanece em determinada área da página
*da passagem do mouse por links e duração da passagem
*do traçado completo do ponteiro
*da correlação com o horário da ação

##### Esse tipo de tecnologia permite a identificação de usuário previamente considerado anônimo, pois cada usuário tem uma maneira de interagir com o mouse e 
páginas web, o que, ao longo do tempo, pode ser utiliado para criar um identificador. Desabilitar o javascript não inibe esse tipo de ataque, que pode ser
realizado, por exemplo, por CSS.

##### A identificação de usuários considerados anônimos também pode ocorrer por meio dos padrões de digitação. A velocidade, o tempo que a tecla fica pressionada,
erros cometidos, probabilidade de ser destro ou canhoto, abreviações utilizadas, comprimento médio de frases, frequência no uso de palavras, pausas na digitação,
dentre outros parâmetros, podem criar uma identidade única para cada pessoa, mesmo com a variabilidade natural da escrita ao longo do dia. 

##### Uma contramedida é não realizar a digitação no navegador, mas em um bloco de notas, posteriormente copiando o texto. Outra alternativa é o bloqueio de
scripts. Essas alternativas, no entanto, não são perfeitas, não eliminando o problema completamente. A tradução por serviços na web também não mitiga o 
anteriormente descrito.

##### Técnicas como essa podem ser utilizadas para identidicar um autor de um texto ou documento anônimo, sendo utilizada inteligência artificial e análise estatística. 

##### Uma forma mais eficaz de mitigação é a cópia do estilo de escrita de outros autores.

### Endereços MAC

##### O endereço Media Access Control (MAC) é um endereço de hardware vinculado às interfaces de rede, como conexões por cabo ou sem fio. Geralmente, um único computador apresenta diversos endereços MAC, um para cada interface.
Dispositivos conectados na mesma rede, ou softwares instalados nesses dispositivos, têm a capacidade de identificar os endereços MAC de todos os demais dispositivos conectadoa à rede, proporcionando a identificação de uso de uma determinada rede por um dispositivo em específico.
Ao longo do tempo, e com a correlação de imagens de câmeras de segurança, é possível, para um adversário tecnologicamente capacitado, identificar as redes às quais o dispositivo se conecta com regularidade e correlacionar com o usuário que realiza essas conexões.

##### Uma contramedida é a randomização do endereço MAC. No linux, pode-se usar o pacote "macchanger", com os seguintes comando no terminal:

##### *ifconfig

##### *sudo macchanger -r (interface que terá o endereço alterado)

### Beacons

##### Beacons são rastreadores presentes em páginas web, anúncios e mensagens de email, capazes de capturar informações como o horário relacionada à abertura do email ou website.
Comumente consistem de pequenas imagens de 1 x 1 pixel, não sendo identificados pelos usuários. Têm capacidade de se conectar a servidores de terceiros, que implantam cookies no navegador do usuário. Esse cookie é reenviado ao servidor quando o usuário navega para outro site que também contenha beacons do mesmo serviço,
o que, ao lngo do tempo, cria um perfil contendo uma grande proporção de hábitos de navegação. 

##### A contramedida mais efetiva é a utilização do Tor Browser.

### History sniffing

##### Na maioria dos navegadores, o histórico e o cache são compartilhados, o que abre margem para ataques de sniffing. Comumente, links visitados são apresentados de formas diferentes dos não visitados. Caso um site com código javascript malicioso seja acessado pelo usuário, o atacante pode criar links para sites diversos em regiões ocultas da página,
utilizando a interface DOM do navegador para inspecionar a forma na qual os links são apresentados, possibilitando revelar os sites previamente acessados. 

##### O uso de CSS (CSS Stylesheets) também pode agravar o problema. A contramedida mais efetiva é a utilização do Tor Browser.

### Session replay scripts

##### Alguns javascripts são denominados “session replay”, ou de reprodução de sessão. Com capacidade de armazenar movimentos do ponteiro, rolagem da página, teclas pressoinadas, dentre outros; possibilita a completa reprodução da sessão do usuário,
com essas informações sendo enviadas para servidores de terceiros. Desabilitar o javascript previne completaemnte esse tipo de ataque. 

### Ultrasssom

##### Por meio de ultrassom, novas técnicas de rastreamento estão surgindo no mercado tecnológico.

##### Um cenário possível é a exibição de propagandas na internet, rádio ou televisão com áudio na frequência ultrassônica oculto, interceptados pelos microfones dos smartphones presentes no ambiente. Caso aplicativos capazes de interpretar as informações presentes no áudio estejam instalados no aparelho móvel,
é possível relacionar os hábitos de consumo de mídia com a identidade do usuário do aparelho celular. 

##### Outra possibilidade é a utilização de ultrassom em anúncios na web, relacionando hábitos de navegação à identidade de usuários de outros dispositivos inteligentes, integrando o rastreamento entre esses dispositivos. 

##### A utilização de ultrassom também pode revelar as identidades de pessoas pŕoximas ao usuário, bem como a frequência de interação. 

##### Uma contramedida é a utilização de aplicativos open source e a restrição de acesso ao microfone aos aplicativos que realmente necesssitam dessa permissão. Uma medida mais extrema é a remoção física dos componentes de hardware em questão. 

##### Existem, ainda, outros métodos de rastreio, porém, não utilizados com tanta frequência, como ataques de correlação utilizados em conexões efetuadas por meio de redes anônimas, como o TOR. Mesmo alguns dos mencionados nesse capítulo não apresentam uso massificado. Apenas adversários mais sofisticados detêm
a capacidade necessária para realizar os mais sofisticados. Quanto mais complexo for o método, menos agentes serão capazes de executar as ações necessárias.
