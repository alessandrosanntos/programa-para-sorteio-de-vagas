Sistema de Sorteio Público Auditável -
COLUNI-UFF
Sobre o Projeto
Este software foi desenvolvido visando garantir transparência, segurança e auditoria no
processo de sorteio público para ingresso de novos alunos no Colégio Universitário
Geraldo Reis (COLUNI-UFF).
O sistema automatiza o sorteio aleatório de candidatos, respeitando rigorosamente as cotas,
a ordem de prioridade e o remanejamento de vagas não preenchidas, conforme as regras de
editais de concursos públicos.
Créditos e Licença
● Desenvolvedor: Alessandro Santos
● GitHub: @alessandrosanntos
● Licença: Código Aberto (Open Source). Este software pode ser copiado, modificado e
distribuído livremente, desde que mantidos os créditos originais.
Funcionalidades Principais
1. Auditoria Robusta:
○ Utiliza uma "Semente de Aleatoriedade" (Seed) manual (ex: número do concurso
da Loteria Federal ou Data/Hora), permitindo que qualquer pessoa reproduza o
sorteio e chegue exatamente ao mesmo resultado.
○ Gera um Hash (assinatura digital) do arquivo de inscritos para provar que a lista
não foi alterada.
○ Gera logs detalhados em .txt e .pdf.
2. Gestão de Vagas e Cotas:
○ Permite definir vagas para Imediata e Cadastro de Reserva separadamente.
○ Cotas suportadas: PPI1, PPI2, RF (Renda Familiar), PCD e AC (Ampla
Concorrência).
○ Remanejamento Automático: Vagas não preenchidas nas cotas são transferidas
automaticamente para a Ampla Concorrência.
3. Interface Visual (GUI):
○ Desenvolvido em Python com Tkinter.
○ Resolução otimizada para 1366x768.
○ Animação para exibição dos sorteados (simulando sorteio presencial).
○ Exibição de planilha de resultados ao final de cada turma.
Estrutura do Arquivo de Dados (base.xlsx)
Para que o sistema funcione, o arquivo Excel deve conter as seguintes colunas na ordem
exata (A a E):
Coluna Nome do Campo Descrição
A Inscrição Número de inscrição do
candidato.
B Nome Nome completo do candidato.
C Turma Turma pretendida (ex: "TURMA
1", "1º ANO EF").
D Cota EI Cota para Educação Infantil.
E Cota EFEM Cota para Ensino
Fundamental/Médio.
Nota: O sistema ignora automaticamente linhas onde o nome seja "NÚMERO CANCELADO".
Requisitos do Sistema
● Sistema Operacional: Windows 10/11, Linux ou macOS.
● Para executar o código fonte:
○ Python 3.8 ou superior.
○ Bibliotecas necessárias: pandas, openpyxl, fpdf.
○ Instalação: pip install pandas openpyxl fpdf
Como Contribuir
Sendo um projeto de código aberto, contribuições são bem-vindas. Sinta-se à vontade para
fazer um fork deste projeto, implementar melhorias e enviar um pull request.
Desenvolvido com
❤ para a educação pública.
