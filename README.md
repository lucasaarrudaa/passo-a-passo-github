# PASSO A PASSO GITHUB

## PRIMEIROS PASSOS

1. Crie um repositório no GitHub.
2. Clone o repositório do GitHub em sua máquina local:
	1. Dentro do repositório no GitHub, clique em "<Code>" e copie a URL. 
	2. Abra o terminal, navegue até o diretório onde você quer que o repositório local seja colocado e digite `git clone <url-do-repositório>`.
3. Agora você pode começar a fazer alterações no seu repositório local. Após realizar as alterações, use `git status` no terminal para visualizar quais arquivos foram modificados.

## CONCEITOS IMPORTANTES

- Pull e Push:
	1. Pull: É a ação de buscar e incorporar alterações de um repositório remoto para o seu repositório local. Para executá-lo, use o comando `git pull origin <nome-da-branch>`.
	2. Push: É a ação de enviar as alterações locais para o repositório remoto. Para executá-lo, use o comando `git push origin <nome-da-branch>`.

- Branch (Ramo):
	Uma branch é basicamente uma versão paralela do código. As branches são usadas para:
		- Desenvolver funcionalidades isoladamente
		- Corrigir bugs sem interferir no desenvolvimento principal
		- Experimentar novas ideias
		- Facilitar revisões de código e pull requests
		- Preparar e manter versões de produção
	Para visualizar sua branch atual, use `git branch`. A branch em que você está atualmente será indicada com um asterisco (*).
	
- Checkout, Switch e Restore:
	1. `git checkout`: Utilizado para alternar entre branches ou para descartar alterações em um arquivo específico.
	2. `git switch`: Introduzido no Git 2.23, este comando é uma maneira mais intuitiva de alternar entre branches.
	3. `git restore`: Também introduzido no Git 2.23, este comando é uma maneira mais clara de descartar alterações em arquivos.

- Staging Area (Área de Preparação):
	É uma área intermediária onde as alterações são agrupadas antes de serem commitadas. Comandos relevantes incluem `git add` (para adicionar alterações à staging area) e `git commit` (para armazenar permanentemente as alterações no repositório).

- Merge (Fusão) e Branching (Ramificação):
	1. Merge: O processo de unir duas ou mais branches. Isso é comumente feito após a conclusão do trabalho em uma branch de feature, quando as alterações estão prontas para serem combinadas de volta à branch principal.
	2. Branching: O processo de criação de uma nova linha de desenvolvimento separada do código principal. Isso é útil para desenvolver novas funcionalidades ou corrigir bugs sem perturbar o código principal.

## FLUXO DE TRABALHO

1. Faça alterações: Por exemplo, você pode adicionar um arquivo chamado `cluster_model.py` ao seu repositório.
2. Adicione as alterações ao Stage: Use `git add cluster_model.py` ou `git add .` para adicionar todas as alterações ao Stage.
3. Commit suas alterações: Use `git commit -m "Adicionando o modelo de clusterização"`.
4. Push suas alterações para o repositório remoto: Use `git push origin master` ou `git push origin main` (dependendo da configuração do seu repositório).
5. Pull as alterações do repositório remoto: Use `git pull origin master` ou `git pull origin main`.
6. Lembre-se de que os comandos git pull e git push devem ser usados na branch que você deseja atualizar ou enviar atualizações.

**NOTA:** Sempre verifique o estado do seu repositório antes de executar comandos. Se você não tiver certeza, use `git status`.
