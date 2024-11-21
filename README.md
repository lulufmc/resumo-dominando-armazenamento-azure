# resumo-dominando-armazenamento-azure
Este repositório contém o resumo sobre o tópico de "Dominando o Armazenamento na Azure"

# Armazenamento

- Armazenamento no Azure

  O armazenamento no Azure é usado para salvar dados de diferentes tipos (arquivos, tabelas, blobs, filas, etc.) de maneira segura, escalável e acessível de qualquer lugar. É um serviço base para aplicativos e infraestruturas.

- Conta de Armazenamento
  
  Uma conta de armazenamento é como uma porta de entrada para acessar todos os serviços de armazenamento no Azure. Deve ter um globalmente nome exclusivo. Fornecer acesso à internet em todo o mundo. E determinar os serviços de armazenamento e as opções de redundância. Dentro de uma conta, você pode ter diferentes tipos de serviços:
  
  • Blobs: Armazenamento de objetos (imagens, vídeos, backups, etc.).
  • Files: configura um compartilhamento de arquivos de rede altamente disponível, que pode ser utilizado usando o protocolo Bloco de Mensagens do Servidor.
  • Queues: Gerenciamento de mensagens para comunicação entre aplicativos.
  • Disco do azure: fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizaram. 
  • Tables: Banco de dados NoSQL para aplicativos leves. Fornece uma opção de chave/atributo para o armazenamento de dados estruturados não relacionais com um design sem esquema.

- Redundância de Armazenamento

  Redundância é a maneira como o Azure garante que seus dados estejam disponíveis e protegidos contra falhas de hardware, interrupções regionais ou desastres. O Azure oferece configurações de redundância diferentes para atender necessidades variadas:
  
  • LRS (Armazenamento com redundância local): Mantém três cópias dos seus dados na mesma região, mas em racks diferentes dentro do mesmo data center. Durabilidade de 11 noves.
  • ZRS (Armazenamento com redundância de zona): Mantém cópias sincronizadas dos dados em três zonas de disponibilidade dentro da mesma região. Durabilidade de 12 noves.
  • GRS (Armazenamento com redundância de geográfica): Mantém cópias dos dados em duas regiões diferentes, uma região principal onde os dados são gravados, e uma região secundária geograficamente distante. Durabilidade de 16 noves.
  • GZRS (Armazenamento com redundância de zona geográfica): Combina a proteção de ZRS (zonas de disponibilidade) e GRS (replicação entre regiões). 3 zonas de disponibilidade na região primária, e um único datacenter na região secundária. Durabilidade de 16 noves.

- Camadas de armazenamento do Azure

  • Frequente: Otimizada para armazenamento de dados acessados com frequência. Menor custo para acesso/consulta dos dados.
  • Esporádico: Otimizada para armazenamento de dados acessados com pouca frequência e armazenados por pelo menos 30 dias. 
  • Frio: Otimizada para armazenamento de dados acessados com pouca frequência, e armazenados por pelo menos 90 dias. 
  • Arquivo morto: Otimizada para armazenamento de dados acessados com pouca frequência, e armazenados por pelo menos 180 dias, com requisitos de latência flexíveis. Maior custo para acesso/consulta dos dados.

- Migrações para o Azure

  Plataforma de migração unificada. Intervalo de ferramentas integradas e autônomas. Avaliação e migração.

  • Azure Data Box: Usado para empresas que querem levar seus datacenters para nuvem, e que possuem grande quantidade de dados. Armazena até 80TB de dados. Move os backups de recuperação de desastre para o Azure. Proteja seus dados em uma caixa robusta durante o trânsito.
  • AzCopy: Utilitário de linha de comando. Copiar blobs ou arquivos de para sua conta de armazenamento. Sincronização em uma única direção.
  • Gerenciador de Armazenamento do Azure: Interface gráfica do usuário(de modo semelhante ao Windows Explorer). Compatível com Windows, MacOS e Linux.
  • Sincronização de Arquivos do Azure: Sincroniza os arquivos do Azure e locais de forma bidirecional. A cama de nuvem mantém os arquivos acessados com frequência no local, enquanto libera espaço.
  
