classDiagram
direction BT
class AparelhoTelefonico {
<<Interface>>
  + desligar() void
  + ligar(String) void
  + atender() void
  + iniciarCorreioVoz() void
  + encerrarChamada() void
}
class Iphone {
  + Iphone() 
  + desligar() void
  + ligar(String) void
  + atender() void
  + tocar() void
  + iniciarCorreioVoz() void
  + adicionarNovaAba() void
  + selecionarMusica(String) void
  + encerrarChamada() void
  + pausar() void
  + atualizarPagina() void
  + exibirPagina(String) void
}
class NavegadorInternet {
<<Interface>>
  + exibirPagina(String) void
  + adicionarNovaAba() void
  + atualizarPagina() void
}
class ReprodutorMusical {
<<Interface>>
  + tocar() void
  + pausar() void
  + selecionarMusica(String) void
}

Iphone  ..>  AparelhoTelefonico 
Iphone  ..>  NavegadorInternet 
Iphone  ..>  ReprodutorMusical 
