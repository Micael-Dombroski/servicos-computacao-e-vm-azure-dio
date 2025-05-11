# Serviços de Computação e VMs do Azure
## Computação e Rede
### Serviços de Computação do Azure
#### Computação do Azure
  Serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e SO.

### Máquinas Virtuais (VMs)
Emulações de software de computader físicos, possuem processador virtual, memória, armazenamento e rede. <br>
Oferta de IaaS que oferece personalização e controle total.

#### Conjuntos de Dimensionamento de VMs
Oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente, escalando horizontalmente quando o recurso precisar aumenter e reduzindo quando precisar diminuir.

#### Conjuntos de Disponibilidade de VMs
Domíonios de falha, cada um fique fora do ar há outros ainda operando. Um domínio de atualização atualiza por vez apenas parte das VMs do conjunto de disponibilidade para o serviço seguir operando.

### Área de Trabalho Virtual do Azure
Uma virtualização de área de trabalho e aplicativo executada na nuvem, não precisa executar outros servidores de gatewat (pois isso é gerenciado pela Microsoft). <br>
Reduz o risco do recurso ser deixado para trás (Funcionário ficando com o PC da empresa após ser demitido xd). <br>
Permite implantações reais de várias sessões.

### Serviços de Contêineres do Azure
Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do SO e pode responder a alterações sob-demanda.

#### Instâncias de Contêiner
Oferta de PaaS que executa um contêiner ou pod de contêineres no Azure.

#### Aplicativos de Contêiner
Oferta de PaaS, como instâncias de contêineres, que pode balancear a carga e escalar.

#### Servidores de Kubernetes do Azure
Serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres. Gerencia o ciclo de vida dos contêineres, em alguns momentos precisa de mais para uma atividade e depois os contêineres extras são descartados.

### Azure Functions
Oferta de PaaS que dá suporte a operações de computação sem servidor. <br>
O código se baseia em eventos e é executado quando chamado, sem exigir infraestrutura de servidor durante períodos inativos. <br>
São dimensionadas automaticamente com base na demanda.

### Comparando opções de computação do Azure
#### VMs
Servidor baseado em nuvem com suporte a ambientes Windows ou Linux. <br>
Útil para migrações de lift-and-shift (leva do jeito que está, sem modernizar) para a nuvem. <br>
Pacode do SO completo, incluindo o SO do host.

#### Área de Trabalho Virtual
Fornece a experiência da área de trabalho do Windows baseada em nuvem. <br>
Aplicativos dedidcados para conexão e uso ou acessíveis de qualquer navegador moderno. <br>
Logon de vários clientes permite que vários usu[arios façam logon no mesmo computador ao mesmo tempo.

#### Contêineres
Ambiente leve e em miniatura, adequado para a execução de microsserviços. <br>
Projeto para escalabilidade e resliência por meio da orquestração. <br>
Aplicativos e serviços são empacotados num contêiner que fica na parte superior do SO do host. Vários contêineres podem ficar num SO do host.

### Serviços de aplicativo do Azure
A Rede Virtual do Azure (VNet) permite que os recursos do Azure se comuniquem uns com os outros, com a internet e com as redes locais. <br>
- Pontos de extremidade públicos são acessíveis de qualquer lugar na internet.
- Pontos de extremidade privados são acessíveis somente dentro da sua rede.
- As sub-redes virtuais segmentam na sua rede para atender às suas necessidades.
- O emparelhamento de rede conecta suas redes privadas diretamente.

#### Gateway de VPN
É usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela Internet pública.

#### Express Route
Conexão direta via cabo, é uma opção viável se a empresa estiver próxima de uma região do Azure. Estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade.

### DNS do Azure (DNS = Domain Name System)
- Confiabilidade e desempenho com uma rede global de servidores de nome DNS usando a rede Anycast.
- Sua segurança se baseia no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log.
- Facilidade de uso para gerencias seus recursos externos e do Azure com um único DNS.
- As redes virtuais personalizáveis permitem que você use nomes de domínio privados e personalizados em suas redes virtuais privadas.
- Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure.
