unit uFrmPrincipal;

interface

uses
  Winapi.Windows, Winapi.Messages, System.SysUtils, System.Variants, System.Classes, Vcl.Graphics,
  Vcl.Controls, Vcl.Forms, Vcl.Dialogs, Vcl.ExtCtrls, Vcl.ComCtrls, Vcl.StdCtrls,
  System.ImageList, Vcl.ImgList;

type
  TFrmPrincipal = class(TForm)
    pnlTitulo: TPanel;
    PagCntrPrincipal: TPageControl;
    TabSheet1: TTabSheet;
    TabSheet2: TTabSheet;
    TabSheet3: TTabSheet;
    GroupBox1: TGroupBox;
    Label1: TLabel;
    EditCaracteres: TEdit;
    BtnExibirDataHora: TButton;
    Lista24x24: TImageList;
    Lista48x48: TImageList;
    procedure pnlTituloClick(Sender: TObject);
    procedure EditCaracteresEnter(Sender: TObject);
    procedure EditCaracteresExit(Sender: TObject);
  private
    { Private declarations }
  public
    { Public declarations }
  end;

var
  FrmPrincipal: TFrmPrincipal;

implementation

{$R *.dfm}

procedure TFrmPrincipal.EditCaracteresEnter(Sender: TObject);
begin
 EditCaracteres.Color := $00B9FFFF;
end;

procedure TFrmPrincipal.EditCaracteresExit(Sender: TObject);
begin
  begin
  if EditCaracteres.Text = '' then
  begin
    MessageDlg('Você não digitou nunhum conteúdo', mtError, [mbOK], 0);
    EditCaracteres.SetFocus;
  end
  else
    if Length(EditCaracteres.Text) <> 4 then
    begin
      MessageDlg('Você não digitou o total de 4 caracteres', mtError, [mbOK], 0);
      EditCaracteres.SetFocus;
      EditCaracteres.SelectAll;
    end
    else
      EditCaracteres.Color := $FFFFFF;
  end ;
end;

procedure TFrmPrincipal.pnlTituloClick(Sender: TObject);
begin
  pnlTitulo.Caption := 'Mudando o caption do Panel com onShow';
  pnlTitulo.Color := $00B9FFFF;
end;

end.
