**Imagem completa para ambiente de desenvolvimento com flutter.**

**Flutter version**: 3.0.1
**Dart version**: 2.17.1

**Pacotes contidos**:
Ubuntu 18.04
curl
git
unzip 
xz-utils 
zip 
libglu1-mesa

**Detalhes sobre as propriedades que usamos dentro do devcontainer.jsonarquivo estão listados abaixo**:

**name** : um nome de exibição para o contêiner.

**context**: O caminho do qual a compilação do Docker deve ser executada em relação a devcontainer.json.

**dockerFile**: a localização de um Dockerfile que define o conteúdo do contêiner. O caminho é relativo ao devcontainer.jsonarquivo.

**remoteUser**: O nome do usuário que será usado no container.

**mounts** : uma matriz com pontos de montagem que devem ser adicionados ao contêiner em tempo de execução. Aqui, montamos /dev/bus/usbpara que o container possa detectar qualquer dispositivo Android conectado ao sistema ( NÃO APLICÁVEL para macOS e Windows ).

**settings**: adiciona valores padrão settings.jsonem um arquivo de configurações específico do contêiner/máquina.

**runArgs**: uma matriz com valores de string que devem ser argumentos válidos do Docker. Usamos --privilegedpara garantir que o contêiner possa acessar os dispositivos conectados ao sistema.

**extensions**: uma matriz de IDs de extensão que especifica as extensões que devem ser instaladas dentro do contêiner quando ele é criado. dart-code.flutteré a extensão oficial para o desenvolvimento do Flutter.

**workspaceMount**: Substitui o ponto de montagem local padrão para o espaço de trabalho.

**workspaceFolder**: define o caminho padrão que o VS Code deve abrir ao se conectar ao contêiner.
