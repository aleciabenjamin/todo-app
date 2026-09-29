## To Do App Anmärkningar

#### Varför är .map ett löpande band?

Data finns i state(todos).
`{todos.map(function (todo) {
					return (
						<li key={todo}>
							{todo}{" "}
							<button
								type="button"
								onClick={function () {
									handleRemove(todos);
								}}`
Som på ett löpande band går .map genom varje todo (data) i arrayen och funktionen tillämpas på varje att todo.

### Varför är .filter en sil och inte en kniv?

En sil sorterar och en kniv ändrar formen. .filter gör inga ändringar utan den släpper igenom vissa saker.

### Vad gör key — och vad är den INTE?

key är ett unikt id per list-syskon så React kan matcha rätt rad när listan ändras. Det är inte synlig text för användaren.\

**Sök filtrerar UI — den muterar inte state-listan.**
