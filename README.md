# Getnet.com
website
cfg.MUI, cfg.Light

function OnStart()

{

    lay = app.CreateLayout("Linear", "VCenter, FillXY");

    lay.SetBackColor( MUI.colors.white );

    btn = MUI.CreateButtonRaised("BUTTON", 0.4, null, MUI.colors.teal.teal);

    lay.AddChild(btn);

    btn = MUI.CreateButtonRaisedO("BUTTON", 0.4, null, MUI.colors.teal.teal);

    lay.AddChild(btn);

    btn = MUI.CreateButtonRound("BUTTON", 0.4, null, MUI.colors.deepPurple.darken1);

    lay.AddChild(btn);

    btn = MUI.CreateButtonRoundO("BUTTON", 0.4, null, MUI.colors.deepPurple.darken1);

    lay.AddChild(btn);

    btn = MUI.CreateButtonElegant("BUTTON", 0.4, null, MUI.colors.blue.darken2);

    lay.AddChild(btn);

    btn = MUI.CreateButtonFlat("BUTTON", 0.4, null, MUI.colors.pink.pink);

    lay.AddChild(btn);

    btn = MUI.CreateButtonToggle("TOGGLE", 0.4, null, true, OnToggle, MUI.colors.green.darken2);

    lay.AddChild(btn);

    app.AddLayout(lay);

}

function OnToggle(val)

{

    app.ShowPopup(val);

}
