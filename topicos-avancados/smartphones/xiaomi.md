# Xiaomi

## Nível básico

O procedimento descrito a seguir, relata o passos realizados em um smartphone da marca Xiaomi, modelo da linha redmi. Similaridades serão encontradas em outros aparelhos Android, contudo.

Durante o primeiro início, ou depois de efetuada a formatação do dispositivo, ao longo das configurações iniciais, pule a etapa de login com sua conta google. Isso reduzirá a quantidade de informações associadas à sua conta. Desmarque, também, a permissão de busca de redes e envio de dados diagnóstico.

No caso da Xiaomi, pule o login da conta MI.

Por fim, desabilite o programa de experiência do usuário e os anúncios personalizados.

Caso o seu dispositivo já estiver em uso e você não deseje formatá-lo, poderá procurar essas opções na barra de busca dentro das configurações do seu aparelho.

Com o dispositivo já configurado e inicializado, entre nas configurações. Vá até "apps" e, depois, "gerenciar apps". Clique em "desinstalar" e faça a desinstalação de todos os aplicativos que não são necessários a você. Ainda em "apps", revise as permissões concedidas para os aplicativos instalados em seu aparelho. Aplicativos como a sua calculadora não necessitam de acesso aos seus contatos, mas tome cuidado para não revogar permissões importantes, principalmente em softwares críticos, como o google play services.

Em configurações, pesquise por autorização e revogação. Revogue a autorização de todos os aplicativos, exceto "atualizações".

Por fim, tenha uma senha forte para entrar em seu celular, não algo como "senha" ou "123", mas algo que impeça alguém de acessar seus dados quando você não estiver por perto.

## Nível intermediário

Ainda em privacidade, desative o "encontre meu dispositivo" e desabilite o "play protect".

Desligue as frequências de rádio que não estiver utilizando, como os dados móveis, bluetooth, redes sem fio e localização. Essas medidas ajudam a reduzir a quantidade de informações compartilhadas por seu dispositivo, contudo, não inibem o problema completamente, pois algumas conexões não necessitam da permissão do usuário para ocorrer.

Em "sobre o telefone", clique repetidamente em "versão do miui", até obter status de desenvolvedor. Volte às configurações e vá em "configurações adicionais", e, em seguida, em "opções de desenvolvedor". Habilite a depuração por USB. Permita e aceite.

Será utilizado o software ADB para a remoção de aplicativos nativos, os bloatwares que vêm junto com o seu aparelho. Aqueles aplicativos que você não usa, mas não consegue desinstalar. Um aviso, apenas desinstale aplicativos que não geram problemas, como os não necessários para o funcionamento do aparelho. Pode ser necessário pesquisar sobre o seu aparelho em específico. Caso acabe desinstalando um aplicativo importante por engano, poderá haver a necessidade de formatar o dispositivo. Me pergunte como eu sei.

A descrição a seguir trata do uso do ADB nas distribuições linux.

Com os passos anteriores executados, conecte o celular ao computador. Abra o terminal de sua distribuição e digite os seguintes comandos:

\*sudo apt install adb

\*adb devices

\*adb shell

**Para desinstalar os aplicativos desejados, utilize o seguinte comando:**

\*pm uninstall -k --user 0 com.miui.analytics

**ou**

\*pm disable-user com.miui.weather2

para desabilitar os aplicativos escolhidos. Nos dois casos, altere a parte final do comando para o pacote de sua escolha. O nome do pacote não é o mesmo do aplicativo. Para descobrir o nome do pacote, abra "configurações" =&gt; "apps" =&gt; "gereciar apps" =&gt; selecione o aplicativo =&gt; clique no "i" no canto superior direito. O nome que você deverá inserir no comando está em "nome do APK".

Contanto que não desinstale aplicativos importantes para o sistema, ou alguns sabidamente problemáticos \(procure nos fóruns relativos ao seu dispostivo\), não haverá grandes problemas. Em todo o caso, é recomendado realizar backup prévio. A escolha pelos aplicativos que desejar desinstalar é subjetiva. No caso da Xiaomi, recomendo desinstalar, principalmente, o "com.miui.analytics" e o "com.miui.msa.global", basicamente, spywares integrados ao sistema.

Quando terminar, para sair, digite exit.

Terminada essa etapa, instale a loja de aplicativos f-droid. Você poderá instalar pelo site do projeto, efetuando o download do APK. Alguns aplicativos desinstalados por você nas etapas anteriores não necessitam de substitutos, contudo, você poderá substituir aplicativos úteis por alternativas presentes no f-droid, como a câmera e o navegador. Os aplicativos sob a denominação "simple tools" são algumas alternativas encontradas para os aplicativos mais comuns presentes nos smartphones. Ainda, um excelente aplicativo para ter em seu dispositivo é o netguard. Com ele, você poderá controlar quais appa terão acesso à internet, o que reduz, por si só, substancialmente a quantidade de informações enviadas por seu dispositivo a servidores remotos espalhados pelo mundo. Como ainda estamos na ROM proprietária do fabricante, essa etapa torna-se ainda mais importante. Nem todos os aplicativos que gostaríamos de desinstalar são realmente possíveis sem quebrar o sistema.

As etapas mencionadas até esse ponto são suficientes para o aumento substancial de sua privacidade em smartphones, todavia, ainda existem alternativas mais atrativas para os que desejam mais privacidade, porém, com maior custo embutido.

## Nível avançado

A desinstalação de aplicativos, a substituição por alternativas mais amigas da privacidade e o bloqueio do acesso à internet, ainda são limitados pela ROM instalada no dispositivo. Existem algumas alternativas de ROMs open source, como o GrapheneOS, CalyxOS e LineageOS. Os dois primeiros, com foco nos aparelhos Pixel, da Google. O último, com ampla gama de aparelhos, como modelos das marcas Google, Samsung, Sony e Xiaomi. Adicionalmente, começam a surgir no mercado, opções de aparelhos celulares com sistemas operacionais Linux, como o PinePhone e o Librem 5, porém, ainda em fase preliminar de desenvolvimento ou venda.

