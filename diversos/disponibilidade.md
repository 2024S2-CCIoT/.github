Planejar o tempo de disponibilidade de uma solução sem um histórico prévio é um desafio comum, especialmente ao iniciar um novo projeto ou migrar uma aplicação para uma nova infraestrutura. 

# Algumas estratégias

### 1. **Entendimento dos Requisitos de Negócio e Usuário**
   - **Identifique as Necessidades do Negócio**: Determine o impacto que a indisponibilidade pode ter sobre o negócio. Pergunte-se quais operações são críticas para o sucesso da empresa. Por exemplo, uma aplicação de e-commerce que processa vendas online terá requisitos de disponibilidade mais altos em comparação com um sistema interno de relatórios.
   - **Estabeleça Expectativas de Usuário**: Compreenda as expectativas dos usuários em relação à disponibilidade. Isso pode envolver benchmarking contra soluções similares ou buscar informações sobre o comportamento típico dos usuários em relação ao uso da aplicação.

### 2. **Análise de Risco e Impacto**
   - **Classifique os Riscos Potenciais**: Avalie os riscos que podem impactar a disponibilidade, como falhas de hardware, interrupções de rede, ataques de segurança, ou problemas com software. Liste esses riscos e atribua uma prioridade a eles com base no impacto potencial sobre a solução.
   - **Determine a Tolerância ao Risco**: Defina o nível de tolerância ao risco para a solução. Em ambientes onde o impacto financeiro de uma interrupção é alto, o objetivo será alcançar uma disponibilidade muito próxima de 100%. Em outros casos, um nível de disponibilidade menor pode ser aceitável.

### 3. **Adote Melhores Práticas de Arquitetura e Infraestrutura**
   - **Escolha uma Arquitetura Resiliente**: Opte por arquiteturas que promovam alta disponibilidade, como arquiteturas redundantes, com failover automático e balanceamento de carga. Utilize componentes que suportem escalabilidade horizontal (como microsserviços) e evite pontos únicos de falha.
   - **Implemente Infraestrutura de Nuvem ou Híbrida**: Considere usar serviços de nuvem que oferecem acordos de nível de serviço (SLAs) com garantias de disponibilidade. Para aplicações críticas, uma infraestrutura híbrida pode ser usada para manter operações críticas on-premises, enquanto aproveita a escalabilidade da nuvem para menos críticas.

### 4. **Planeje Manutenção Proativa**
   - **Automatize Atualizações e Patches**: Estabeleça um cronograma regular de manutenção preventiva para minimizar riscos de falhas não planejadas. Automatize o processo de aplicação de patches e atualizações de software para reduzir o tempo de inatividade.
   - **Monitore Proativamente**: Configure monitoramento para detectar falhas potenciais antes que elas ocorram, e use alertas em tempo real para problemas críticos. Ferramentas de monitoramento de infraestrutura, aplicações, e logs podem ajudar a identificar problemas emergentes.

### 5. **Utilize Simulações e Testes de Falhas**
   - **Realize Testes de Resiliência**: Simule falhas e interrupções para entender como a infraestrutura se comporta. Exercícios como "Game Days" e "Chaos Engineering" podem ajudar a identificar e corrigir pontos fracos.
   - **Teste Regularmente Planos de Recuperação**: Desenvolva e teste planos de recuperação de desastres e procedimentos de backup regularmente para garantir que eles sejam eficazes e atualizados.

### 6. **Baseie-se em Benchmarking e Melhores Práticas**
   - **Estude Casos Similares**: Pesquise como outras organizações com requisitos similares de negócios e usuários planejam sua disponibilidade. Benchmarks da indústria podem fornecer um ponto de partida para estabelecer metas de disponibilidade.
   - **Referências de SLAs Padrão de Mercado**: Examine SLAs oferecidos por provedores de serviços na nuvem (como AWS, Azure, ou Google Cloud) para serviços comparáveis. Esses SLAs geralmente são baseados em anos de dados de operação e podem fornecer um bom ponto de partida.

### 7. **Estabeleça Metas Inicialmente Conservadoras**
   - **Defina Metas Realistas de Disponibilidade**: Sem um histórico, comece com uma meta de disponibilidade que seja conservadora e ajuste conforme o sistema amadurece. Por exemplo, uma meta inicial de 99,9% (equivalente a até 8h 45min de downtime por ano) pode ser ajustada com base em feedback e monitoramento.

### 8. **Documente e Revise Regularmente**
   - **Documente o Plano de Disponibilidade**: Crie documentação que detalhe o planejamento de disponibilidade, incluindo metas, SLAs internos, e planos de recuperação. Revise essa documentação regularmente com base em novos dados operacionais e de uso.

### Conclusão
Sem um histórico, a estratégia é combinar conhecimento sobre as necessidades do negócio e dos usuários, usar práticas comprovadas de arquitetura e infraestrutura, e fazer ajustes constantes baseados em dados coletados de operações e testes. Com o tempo, esse plano será refinado para atender às necessidades específicas da solução.