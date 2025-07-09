# filme
filme
class Filme:
    def __init__(self, titulo, ano, genero, duracao, sinopse, trailer):
        self.titulo = titulo
        self.ano = ano
        self.genero = genero
        self.duracao = duracao
        self.sinopse = sinopse
        self.trailer = trailer  # Link do trailer

    def __str__(self):
        return (f"{self.titulo} ({self.ano}) - {self.genero} - {self.duracao} min\n"
                f"Sinopse: {self.sinopse}\n"
                f"Trailer: {self.trailer}\n")

class CatalogoDeFilmes:
    def __init__(self):
        self.filmes = []

    def adicionar_filme(self, filme):
        self.filmes.append(filme)

    def listar_filmes(self):
        for filme in self.filmes:
            print(filme)
