-- Código salvo em uma URL ou pastebin
local Library = {}

-- Função para criar aba
function Library:CreateKeySystem()
	-- Gui to Lua
	-- Version: 3.2

	-- Instances:

	local PoltergeistKeySystem = Instance.new("ScreenGui")
	local Notifications = Instance.new("Frame")
	local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
	local UIListLayout = Instance.new("UIListLayout")
	local CanvasGroup = Instance.new("CanvasGroup")
	local Topbar = Instance.new("Frame")
	local Title = Instance.new("TextLabel")
	local Padding = Instance.new("UIPadding")
	local TextSize = Instance.new("UITextSizeConstraint")
	local Close = Instance.new("TextButton")
	local Ratio = Instance.new("UIAspectRatioConstraint")
	local Corner = Instance.new("UICorner")
	local Icon = Instance.new("ImageLabel")
	local Constraint = Instance.new("UISizeConstraint")
	local Scale = Instance.new("UIScale")
	local Corner_2 = Instance.new("UICorner")
	local Constraint_2 = Instance.new("UISizeConstraint")
	local Ratio_2 = Instance.new("UIAspectRatioConstraint")
	local Dots = Instance.new("ImageLabel")
	local Key = Instance.new("Frame")
	local Title_2 = Instance.new("TextLabel")
	local Padding_2 = Instance.new("UIPadding")
	local TextSize_2 = Instance.new("UITextSizeConstraint")
	local Key_2 = Instance.new("Frame")
	local UICorner = Instance.new("UICorner")
	local TextBox = Instance.new("TextBox")
	local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")
	local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
	local Asterisco = Instance.new("TextLabel")
	local Padding_3 = Instance.new("UIPadding")
	local TextSize_3 = Instance.new("UITextSizeConstraint")
	local UseKey = Instance.new("TextButton")
	local UICorner_2 = Instance.new("UICorner")
	local UIAspectRatioConstraint_4 = Instance.new("UIAspectRatioConstraint")
	local TextBox_2 = Instance.new("TextLabel")
	local UIAspectRatioConstraint_5 = Instance.new("UIAspectRatioConstraint")
	local Login = Instance.new("Frame")
	local Title_3 = Instance.new("TextLabel")
	local Padding_4 = Instance.new("UIPadding")
	local TextSize_4 = Instance.new("UITextSizeConstraint")
	local AccountName = Instance.new("Frame")
	local UICorner_3 = Instance.new("UICorner")
	local TextBox_3 = Instance.new("TextBox")
	local UIAspectRatioConstraint_6 = Instance.new("UIAspectRatioConstraint")
	local UIAspectRatioConstraint_7 = Instance.new("UIAspectRatioConstraint")
	local Asterisco_2 = Instance.new("TextLabel")
	local Padding_5 = Instance.new("UIPadding")
	local TextSize_5 = Instance.new("UITextSizeConstraint")
	local AccountPassword = Instance.new("Frame")
	local UICorner_4 = Instance.new("UICorner")
	local TextBox_4 = Instance.new("TextBox")
	local UIAspectRatioConstraint_8 = Instance.new("UIAspectRatioConstraint")
	local UIAspectRatioConstraint_9 = Instance.new("UIAspectRatioConstraint")
	local Asterisco_3 = Instance.new("TextLabel")
	local Padding_6 = Instance.new("UIPadding")
	local TextSize_6 = Instance.new("UITextSizeConstraint")
	local Login_2 = Instance.new("TextButton")
	local UICorner_5 = Instance.new("UICorner")
	local UIAspectRatioConstraint_10 = Instance.new("UIAspectRatioConstraint")
	local TextBox_5 = Instance.new("TextLabel")
	local UIAspectRatioConstraint_11 = Instance.new("UIAspectRatioConstraint")
	local Navigation = Instance.new("Frame")
	local MainLoader = Instance.new("TextButton")
	local UICorner_6 = Instance.new("UICorner")
	local UIAspectRatioConstraint_12 = Instance.new("UIAspectRatioConstraint")
	local TextBox_6 = Instance.new("TextLabel")
	local UIAspectRatioConstraint_13 = Instance.new("UIAspectRatioConstraint")
	local KeyStatus = Instance.new("TextLabel")
	local Padding_7 = Instance.new("UIPadding")
	local TextSize_7 = Instance.new("UITextSizeConstraint")

	--Properties:

	PoltergeistKeySystem.Name = "PoltergeistKeySystem"
	PoltergeistKeySystem.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
	PoltergeistKeySystem.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	PoltergeistKeySystem.ResetOnSpawn = false

	Notifications.Name = "Notifications"
	Notifications.Parent = PoltergeistKeySystem
	Notifications.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Notifications.BackgroundTransparency = 1.000
	Notifications.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Notifications.BorderSizePixel = 0
	Notifications.Position = UDim2.new(0.842465758, 0, 0, 0)
	Notifications.Size = UDim2.new(0.157534242, 0, 0.983079553, 0)

	UIAspectRatioConstraint.Parent = Notifications
	UIAspectRatioConstraint.AspectRatio = 0.356

	UIListLayout.Parent = Notifications
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout.VerticalAlignment = Enum.VerticalAlignment.Bottom

	CanvasGroup.Name = "CanvasGroup"
	CanvasGroup.Parent = PoltergeistKeySystem
	CanvasGroup.AnchorPoint = Vector2.new(0.5, 0.5)
	CanvasGroup.BackgroundColor3 = Color3.fromRGB(29, 29, 29)
	CanvasGroup.BorderColor3 = Color3.fromRGB(0, 0, 0)
	CanvasGroup.BorderSizePixel = 0
	CanvasGroup.ClipsDescendants = true
	CanvasGroup.Position = UDim2.new(0.5, 0, 0.499153972, 0)
	CanvasGroup.Size = UDim2.new(0.557617962, 0, 0.781049132, 0)

	Topbar.Name = "Topbar"
	Topbar.Parent = CanvasGroup
	Topbar.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
	Topbar.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Topbar.BorderSizePixel = 0
	Topbar.Position = UDim2.new(0, 0, 2.15154952e-08, 0)
	Topbar.Size = UDim2.new(1, 0, 0.106159054, 0)
	Topbar.ZIndex = 2

	Title.Name = "Title"
	Title.Parent = Topbar
	Title.AnchorPoint = Vector2.new(0, 0.5)
	Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Title.BackgroundTransparency = 1.000
	Title.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Title.BorderSizePixel = 0
	Title.Position = UDim2.new(0, 0, 0.5, 0)
	Title.Size = UDim2.new(0.400000006, 0, 0.375, 0)
	Title.Font = Enum.Font.SourceSansBold
	Title.Text = "POLTERGEIST KEY SYSTEM"
	Title.TextColor3 = Color3.fromRGB(100, 167, 239)
	Title.TextScaled = true
	Title.TextSize = 14.000
	Title.TextTransparency = 0.500
	Title.TextWrapped = true
	Title.TextXAlignment = Enum.TextXAlignment.Left

	Padding.Name = "Padding"
	Padding.Parent = Title
	Padding.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize.Name = "TextSize"
	TextSize.Parent = Title
	TextSize.MaxTextSize = 30

	Close.Name = "Close"
	Close.Parent = Topbar
	Close.AnchorPoint = Vector2.new(0.5, 0.5)
	Close.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Close.BackgroundTransparency = 0.850
	Close.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Close.BorderSizePixel = 0
	Close.Position = UDim2.new(0.972466111, -10, 0.50000006, 0)
	Close.Size = UDim2.new(0.600000024, 0, 0.600000024, 0)
	Close.AutoButtonColor = false
	Close.Font = Enum.Font.SourceSans
	Close.Text = ""
	Close.TextColor3 = Color3.fromRGB(0, 0, 0)
	Close.TextSize = 14.000
	Close.TextTransparency = 1.000

	Ratio.Name = "Ratio"
	Ratio.Parent = Close

	Corner.CornerRadius = UDim.new(1, 0)
	Corner.Name = "Corner"
	Corner.Parent = Close

	Icon.Name = "Icon"
	Icon.Parent = Close
	Icon.AnchorPoint = Vector2.new(0.5, 0.5)
	Icon.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Icon.BackgroundTransparency = 1.000
	Icon.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Icon.BorderSizePixel = 0
	Icon.Position = UDim2.new(0.5, 0, 0.5, 0)
	Icon.Size = UDim2.new(0.600000024, 0, 0.600000024, 0)
	Icon.Image = "rbxassetid://130426375254962"
	Icon.ImageColor3 = Color3.fromRGB(0, 0, 0)
	Icon.ImageTransparency = 0.700

	Constraint.Name = "Constraint"
	Constraint.Parent = Close
	Constraint.MaxSize = Vector2.new(35, 35)

	Scale.Name = "Scale"
	Scale.Parent = Close

	Corner_2.CornerRadius = UDim.new(0.0399999991, 0)
	Corner_2.Name = "Corner"
	Corner_2.Parent = CanvasGroup

	Constraint_2.Name = "Constraint"
	Constraint_2.Parent = CanvasGroup
	Constraint_2.MinSize = Vector2.new(250, 250)

	Ratio_2.Name = "Ratio"
	Ratio_2.Parent = CanvasGroup
	Ratio_2.AspectRatio = 1.350

	Dots.Name = "Dots"
	Dots.Parent = CanvasGroup
	Dots.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
	Dots.BackgroundTransparency = 1.000
	Dots.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Dots.BorderSizePixel = 0
	Dots.Position = UDim2.new(-0.101539157, 0, -0.306836516, 0)
	Dots.Rotation = 45.000
	Dots.Size = UDim2.new(1.20869482, 0, 1.62125564, 0)
	Dots.Image = "rbxassetid://6803353442"
	Dots.ImageTransparency = 0.900
	Dots.ScaleType = Enum.ScaleType.Tile
	Dots.TileSize = UDim2.new(0, 30, 0, 30)

	Key.Name = "Key"
	Key.Parent = CanvasGroup
	Key.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Key.BackgroundTransparency = 1.000
	Key.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Key.BorderSizePixel = 0
	Key.Position = UDim2.new(0, 0, 0.106152475, 0)
	Key.Size = UDim2.new(0, 623, 0, 361)
	Key.Visible = false

	Title_2.Name = "Title"
	Title_2.Parent = Key
	Title_2.AnchorPoint = Vector2.new(0, 0.5)
	Title_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Title_2.BackgroundTransparency = 1.000
	Title_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Title_2.BorderSizePixel = 0
	Title_2.Position = UDim2.new(-0.0144392233, 0, 0.110355072, 0)
	Title_2.Size = UDim2.new(0.451319903, 0, 0.177859664, 0)
	Title_2.Font = Enum.Font.SourceSansBold
	Title_2.Text = "WELCOME BACK, PLAYER!"
	Title_2.TextColor3 = Color3.fromRGB(100, 167, 239)
	Title_2.TextScaled = true
	Title_2.TextSize = 14.000
	Title_2.TextTransparency = 0.500
	Title_2.TextWrapped = true
	Title_2.TextXAlignment = Enum.TextXAlignment.Left

	Padding_2.Name = "Padding"
	Padding_2.Parent = Title_2
	Padding_2.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_2.Name = "TextSize"
	TextSize_2.Parent = Title_2
	TextSize_2.MaxTextSize = 30

	Key_2.Name = "Key"
	Key_2.Parent = Key
	Key_2.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
	Key_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Key_2.BorderSizePixel = 0
	Key_2.Position = UDim2.new(0.0321030244, 0, 0.243767306, 0)
	Key_2.Size = UDim2.new(0.300160527, 0, 0.116343491, 0)

	UICorner.CornerRadius = UDim.new(0, 16)
	UICorner.Parent = Key_2

	TextBox.Parent = Key_2
	TextBox.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox.BackgroundTransparency = 1.000
	TextBox.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox.BorderSizePixel = 0
	TextBox.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox.Size = UDim2.new(0.86096257, 0, 0.571428597, 0)
	TextBox.Font = Enum.Font.Unknown
	TextBox.PlaceholderColor3 = Color3.fromRGB(58, 58, 58)
	TextBox.PlaceholderText = "Key"
	TextBox.Text = ""
	TextBox.TextColor3 = Color3.fromRGB(132, 132, 132)
	TextBox.TextSize = 14.000
	TextBox.TextXAlignment = Enum.TextXAlignment.Left

	UIAspectRatioConstraint_2.Parent = TextBox
	UIAspectRatioConstraint_2.AspectRatio = 6.708

	UIAspectRatioConstraint_3.Parent = Key_2
	UIAspectRatioConstraint_3.AspectRatio = 4.452

	Asterisco.Name = "Asterisco"
	Asterisco.Parent = Key_2
	Asterisco.AnchorPoint = Vector2.new(0, 0.5)
	Asterisco.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Asterisco.BackgroundTransparency = 1.000
	Asterisco.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Asterisco.BorderSizePixel = 0
	Asterisco.Position = UDim2.new(0.856815398, 0, 0.377323508, 0)
	Asterisco.Size = UDim2.new(0.111098655, 0, 0.436353058, 0)
	Asterisco.ZIndex = 3
	Asterisco.Font = Enum.Font.Unknown
	Asterisco.Text = "*"
	Asterisco.TextColor3 = Color3.fromRGB(132, 132, 132)
	Asterisco.TextScaled = true
	Asterisco.TextSize = 100.000
	Asterisco.TextTransparency = 0.500
	Asterisco.TextWrapped = true

	Padding_3.Name = "Padding"
	Padding_3.Parent = Asterisco
	Padding_3.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_3.Name = "TextSize"
	TextSize_3.Parent = Asterisco
	TextSize_3.MaxTextSize = 30

	UseKey.Name = "UseKey"
	UseKey.Parent = Key
	UseKey.Active = false
	UseKey.BackgroundColor3 = Color3.fromRGB(32, 229, 18)
	UseKey.BorderColor3 = Color3.fromRGB(0, 0, 0)
	UseKey.BorderSizePixel = 0
	UseKey.Position = UDim2.new(0.0289007835, 0, 0.389842063, 0)
	UseKey.Selectable = false
	UseKey.Size = UDim2.new(0.259398401, 0, 1.22044122, 0)
	UseKey.Text = ""
	UseKey.TextTransparency = 1.000

	UICorner_2.CornerRadius = UDim.new(0, 16)
	UICorner_2.Parent = UseKey

	UIAspectRatioConstraint_4.Parent = UseKey
	UIAspectRatioConstraint_4.AspectRatio = 4.452

	TextBox_2.Name = "TextBox"
	TextBox_2.Parent = UseKey
	TextBox_2.Active = true
	TextBox_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_2.BackgroundTransparency = 1.000
	TextBox_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox_2.BorderSizePixel = 0
	TextBox_2.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox_2.Selectable = true
	TextBox_2.Size = UDim2.new(0.86096251, 0, 0.571428597, 0)
	TextBox_2.Font = Enum.Font.SourceSansBold
	TextBox_2.Text = "USE KEY"
	TextBox_2.TextColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_2.TextScaled = true
	TextBox_2.TextSize = 14.000
	TextBox_2.TextWrapped = true

	UIAspectRatioConstraint_5.Parent = TextBox_2
	UIAspectRatioConstraint_5.AspectRatio = 6.708

	Login.Name = "Login"
	Login.Parent = CanvasGroup
	Login.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Login.BackgroundTransparency = 1.000
	Login.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Login.BorderSizePixel = 0
	Login.Position = UDim2.new(0, 0, 0.106152475, 0)
	Login.Size = UDim2.new(0, 623, 0, 361)

	Title_3.Name = "Title"
	Title_3.Parent = Login
	Title_3.AnchorPoint = Vector2.new(0, 0.5)
	Title_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Title_3.BackgroundTransparency = 1.000
	Title_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Title_3.BorderSizePixel = 0
	Title_3.Position = UDim2.new(-0.0144392233, 0, 0.110355072, 0)
	Title_3.Size = UDim2.new(0.451319903, 0, 0.177859664, 0)
	Title_3.Font = Enum.Font.SourceSansBold
	Title_3.Text = "LOGIN POLTERGEIST HUB"
	Title_3.TextColor3 = Color3.fromRGB(100, 167, 239)
	Title_3.TextScaled = true
	Title_3.TextSize = 14.000
	Title_3.TextTransparency = 0.500
	Title_3.TextWrapped = true
	Title_3.TextXAlignment = Enum.TextXAlignment.Left

	Padding_4.Name = "Padding"
	Padding_4.Parent = Title_3
	Padding_4.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_4.Name = "TextSize"
	TextSize_4.Parent = Title_3
	TextSize_4.MaxTextSize = 30

	AccountName.Name = "AccountName"
	AccountName.Parent = Login
	AccountName.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
	AccountName.BorderColor3 = Color3.fromRGB(0, 0, 0)
	AccountName.BorderSizePixel = 0
	AccountName.Position = UDim2.new(0.0369184315, 0, 0.401662052, 0)
	AccountName.Size = UDim2.new(0.300160527, 0, 0.116343491, 0)

	UICorner_3.CornerRadius = UDim.new(0, 16)
	UICorner_3.Parent = AccountName

	TextBox_3.Parent = AccountName
	TextBox_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_3.BackgroundTransparency = 1.000
	TextBox_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox_3.BorderSizePixel = 0
	TextBox_3.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox_3.Size = UDim2.new(0.86096257, 0, 0.571428597, 0)
	TextBox_3.Font = Enum.Font.Unknown
	TextBox_3.PlaceholderColor3 = Color3.fromRGB(58, 58, 58)
	TextBox_3.PlaceholderText = "Name Account"
	TextBox_3.Text = ""
	TextBox_3.TextColor3 = Color3.fromRGB(132, 132, 132)
	TextBox_3.TextSize = 14.000
	TextBox_3.TextXAlignment = Enum.TextXAlignment.Left

	UIAspectRatioConstraint_6.Parent = TextBox_3
	UIAspectRatioConstraint_6.AspectRatio = 6.708

	UIAspectRatioConstraint_7.Parent = AccountName
	UIAspectRatioConstraint_7.AspectRatio = 4.452

	Asterisco_2.Name = "Asterisco"
	Asterisco_2.Parent = AccountName
	Asterisco_2.AnchorPoint = Vector2.new(0, 0.5)
	Asterisco_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Asterisco_2.BackgroundTransparency = 1.000
	Asterisco_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Asterisco_2.BorderSizePixel = 0
	Asterisco_2.Position = UDim2.new(0.856815398, 0, 0.377323508, 0)
	Asterisco_2.Size = UDim2.new(0.111098655, 0, 0.436353058, 0)
	Asterisco_2.ZIndex = 3
	Asterisco_2.Font = Enum.Font.Unknown
	Asterisco_2.Text = "*"
	Asterisco_2.TextColor3 = Color3.fromRGB(132, 132, 132)
	Asterisco_2.TextScaled = true
	Asterisco_2.TextSize = 100.000
	Asterisco_2.TextTransparency = 0.500
	Asterisco_2.TextWrapped = true

	Padding_5.Name = "Padding"
	Padding_5.Parent = Asterisco_2
	Padding_5.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_5.Name = "TextSize"
	TextSize_5.Parent = Asterisco_2
	TextSize_5.MaxTextSize = 30

	AccountPassword.Name = "AccountPassword"
	AccountPassword.Parent = Login
	AccountPassword.BackgroundColor3 = Color3.fromRGB(44, 44, 44)
	AccountPassword.BorderColor3 = Color3.fromRGB(0, 0, 0)
	AccountPassword.BorderSizePixel = 0
	AccountPassword.Position = UDim2.new(0.0369184315, 0, 0.540166199, 0)
	AccountPassword.Size = UDim2.new(0.300160527, 0, 0.116343491, 0)

	UICorner_4.CornerRadius = UDim.new(0, 16)
	UICorner_4.Parent = AccountPassword

	TextBox_4.Parent = AccountPassword
	TextBox_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_4.BackgroundTransparency = 1.000
	TextBox_4.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox_4.BorderSizePixel = 0
	TextBox_4.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox_4.Size = UDim2.new(0.86096251, 0, 0.571428597, 0)
	TextBox_4.Font = Enum.Font.Unknown
	TextBox_4.PlaceholderColor3 = Color3.fromRGB(58, 58, 58)
	TextBox_4.PlaceholderText = "Password"
	TextBox_4.Text = ""
	TextBox_4.TextColor3 = Color3.fromRGB(132, 132, 132)
	TextBox_4.TextSize = 14.000
	TextBox_4.TextXAlignment = Enum.TextXAlignment.Left

	UIAspectRatioConstraint_8.Parent = TextBox_4
	UIAspectRatioConstraint_8.AspectRatio = 6.708

	UIAspectRatioConstraint_9.Parent = AccountPassword
	UIAspectRatioConstraint_9.AspectRatio = 4.452

	Asterisco_3.Name = "Asterisco"
	Asterisco_3.Parent = AccountPassword
	Asterisco_3.AnchorPoint = Vector2.new(0, 0.5)
	Asterisco_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Asterisco_3.BackgroundTransparency = 1.000
	Asterisco_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Asterisco_3.BorderSizePixel = 0
	Asterisco_3.Position = UDim2.new(0.856815398, 0, 0.377323508, 0)
	Asterisco_3.Size = UDim2.new(0.111098655, 0, 0.436353058, 0)
	Asterisco_3.ZIndex = 3
	Asterisco_3.Font = Enum.Font.Unknown
	Asterisco_3.Text = "*"
	Asterisco_3.TextColor3 = Color3.fromRGB(132, 132, 132)
	Asterisco_3.TextScaled = true
	Asterisco_3.TextSize = 100.000
	Asterisco_3.TextTransparency = 0.500
	Asterisco_3.TextWrapped = true

	Padding_6.Name = "Padding"
	Padding_6.Parent = Asterisco_3
	Padding_6.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_6.Name = "TextSize"
	TextSize_6.Parent = Asterisco_3
	TextSize_6.MaxTextSize = 30

	Login_2.Name = "Login"
	Login_2.Parent = Login
	Login_2.Active = false
	Login_2.BackgroundColor3 = Color3.fromRGB(32, 229, 18)
	Login_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Login_2.BorderSizePixel = 0
	Login_2.Position = UDim2.new(0.0626006126, 0, 0.681440473, 0)
	Login_2.Selectable = false
	Login_2.Size = UDim2.new(0.24879615, 0, 0.10803324, 0)
	Login_2.Text = ""
	Login_2.TextTransparency = 1.000

	UICorner_5.CornerRadius = UDim.new(0, 16)
	UICorner_5.Parent = Login_2

	UIAspectRatioConstraint_10.Parent = Login_2
	UIAspectRatioConstraint_10.AspectRatio = 4.452

	TextBox_5.Name = "TextBox"
	TextBox_5.Parent = Login_2
	TextBox_5.Active = true
	TextBox_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_5.BackgroundTransparency = 1.000
	TextBox_5.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox_5.BorderSizePixel = 0
	TextBox_5.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox_5.Selectable = true
	TextBox_5.Size = UDim2.new(0.86096251, 0, 0.571428597, 0)
	TextBox_5.Font = Enum.Font.SourceSansBold
	TextBox_5.Text = "Log in"
	TextBox_5.TextColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_5.TextScaled = true
	TextBox_5.TextSize = 14.000
	TextBox_5.TextWrapped = true

	UIAspectRatioConstraint_11.Parent = TextBox_5
	UIAspectRatioConstraint_11.AspectRatio = 6.708

	Navigation.Name = "Navigation"
	Navigation.Parent = CanvasGroup
	Navigation.Active = true
	Navigation.AnchorPoint = Vector2.new(0, 1)
	Navigation.BackgroundColor3 = Color3.fromRGB(39, 39, 39)
	Navigation.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Navigation.BorderSizePixel = 0
	Navigation.Position = UDim2.new(0, 0, 1.00000012, 0)
	Navigation.Size = UDim2.new(1, 0, 0, 0)
	Navigation.ZIndex = 2

	MainLoader.Name = "MainLoader"
	MainLoader.Parent = Navigation
	MainLoader.Active = false
	MainLoader.BackgroundColor3 = Color3.fromRGB(32, 229, 18)
	MainLoader.BorderColor3 = Color3.fromRGB(0, 0, 0)
	MainLoader.BorderSizePixel = 0
	MainLoader.Position = UDim2.new(0.0321110375, 0, 0.134994417, 0)
	MainLoader.Selectable = false
	MainLoader.Size = UDim2.new(0.259398401, 0, 1.22044122, 0)
	MainLoader.Text = ""
	MainLoader.TextTransparency = 1.000

	UICorner_6.CornerRadius = UDim.new(0, 16)
	UICorner_6.Parent = MainLoader

	UIAspectRatioConstraint_12.Parent = MainLoader
	UIAspectRatioConstraint_12.AspectRatio = 4.452

	TextBox_6.Name = "TextBox"
	TextBox_6.Parent = MainLoader
	TextBox_6.Active = true
	TextBox_6.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_6.BackgroundTransparency = 1.000
	TextBox_6.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TextBox_6.BorderSizePixel = 0
	TextBox_6.Position = UDim2.new(0.0695187151, 0, 0.214285716, 0)
	TextBox_6.Selectable = true
	TextBox_6.Size = UDim2.new(0.86096251, 0, 0.571428597, 0)
	TextBox_6.Font = Enum.Font.SourceSansBold
	TextBox_6.Text = "OPEN HUB"
	TextBox_6.TextColor3 = Color3.fromRGB(255, 255, 255)
	TextBox_6.TextScaled = true
	TextBox_6.TextSize = 14.000
	TextBox_6.TextWrapped = true

	UIAspectRatioConstraint_13.Parent = TextBox_6
	UIAspectRatioConstraint_13.AspectRatio = 6.708

	KeyStatus.Name = "KeyStatus"
	KeyStatus.Parent = Navigation
	KeyStatus.AnchorPoint = Vector2.new(0, 0.5)
	KeyStatus.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	KeyStatus.BackgroundTransparency = 1.000
	KeyStatus.BorderColor3 = Color3.fromRGB(0, 0, 0)
	KeyStatus.BorderSizePixel = 0
	KeyStatus.Position = UDim2.new(0.674069881, 0, 0.671199381, 0)
	KeyStatus.Size = UDim2.new(0.295698911, 0, 0.310279369, 0)
	KeyStatus.Font = Enum.Font.SourceSansBold
	KeyStatus.Text = "KEY STATUS: VALID"
	KeyStatus.TextColor3 = Color3.fromRGB(125, 250, 0)
	KeyStatus.TextScaled = true
	KeyStatus.TextSize = 14.000
	KeyStatus.TextTransparency = 0.500
	KeyStatus.TextWrapped = true
	KeyStatus.TextXAlignment = Enum.TextXAlignment.Right

	Padding_7.Name = "Padding"
	Padding_7.Parent = KeyStatus
	Padding_7.PaddingLeft = UDim.new(0.100000001, 0)

	TextSize_7.Name = "TextSize"
	TextSize_7.Parent = KeyStatus
	TextSize_7.MaxTextSize = 30
	
	local Template = Instance.new("CanvasGroup")
	Template.Name = "Template"
	Template.BorderSizePixel = 0
	Template.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Template.AutomaticSize = Enum.AutomaticSize.Y
	Template.Size = UDim2.new(0.96, 0.00, 0.13, 0.00)
	Template.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Template.Position = UDim2.new(1.00, 0.00, 1.00, 0.00)
	Template.Parent = CanvasGroup

	local Frame = Instance.new("Frame")
	Frame.AutomaticSize = Enum.AutomaticSize.Y
	Frame.Size = UDim2.new(1.00, -25.00, 1.00, 0.00)
	Frame.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Frame.Position = UDim2.new(0.00, 15.00, 0.00, 0.00)
	Frame.BorderSizePixel = 0
	Frame.ZIndex = 2
	Frame.BackgroundTransparency = 1
	Frame.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Frame.Parent = Template

	local UIListLayout = Instance.new("UIListLayout")
	UIListLayout.VerticalAlignment = Enum.VerticalAlignment.Center
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout.Parent = Frame

	local Title = Instance.new("TextLabel")
	Title.Name = "Title"
	Title.TextWrapped = true
	Title.ZIndex = 2
	Title.BorderSizePixel = 0
	Title.RichText = true
	Title.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title.AnchorPoint = Vector2.new(0.50, 0.00)
	Title.TextXAlignment = Enum.TextXAlignment.Left
	Title.TextSize = 16
	Title.Size = UDim2.new(1.00, 0.00, 0.00, 10.00)
	Title.Text = "Title"
	Title.TextColor3 = Color3.new(0.41, 0.41, 0.41)
	Title.AutomaticSize = Enum.AutomaticSize.Y
	Title.BackgroundTransparency = 1
	Title.Position = UDim2.new(0.50, 0.00, -0.52, 15.00)
	Title.Parent = Frame

	local Description = Instance.new("TextLabel")
	Description.Name = "Description"
	Description.TextWrapped = true
	Description.ZIndex = 2
	Description.BorderSizePixel = 0
	Description.RichText = true
	Description.TextYAlignment = Enum.TextYAlignment.Top
	Description.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Description.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Medium, Enum.FontStyle.Normal)
	Description.TextTransparency = 0.15000000596046448
	Description.AnchorPoint = Vector2.new(0.50, 0.50)
	Description.TextXAlignment = Enum.TextXAlignment.Left
	Description.TextSize = 14
	Description.Size = UDim2.new(1.00, 0.00, 0.00, 5.00)
	Description.Text = "Description"
	Description.TextColor3 = Color3.new(0.47, 0.47, 0.47)
	Description.AutomaticSize = Enum.AutomaticSize.Y
	Description.BackgroundTransparency = 1
	Description.Position = UDim2.new(0.56, 0.00, 0.50, 7.00)
	Description.Parent = Frame

	local UIPadding = Instance.new("UIPadding")
	UIPadding.PaddingBottom = UDim.new(0.00, 16.00)
	UIPadding.PaddingTop = UDim.new(0.00, 16.00)
	UIPadding.Parent = Frame

	local Interact = Instance.new("TextButton")
	Interact.Name = "Interact"
	Interact.ZIndex = 5
	Interact.BorderSizePixel = 0
	Interact.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Interact.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Interact.AnchorPoint = Vector2.new(0.50, 0.50)
	Interact.TextSize = 14
	Interact.Size = UDim2.new(1.00, 0.00, 1.00, 0.00)
	Interact.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Interact.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Interact.Text = ""
	Interact.BackgroundTransparency = 1
	Interact.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Interact.Parent = Template

	local Shadow = Instance.new("UIStroke")
	Shadow.Name = "Shadow"
	Shadow.Color = Color3.new(0.33, 0.33, 0.33)
	Shadow.Thickness = 1.2000000476837158
	Shadow.Transparency = 1
	Shadow.Parent = Template

	local UICorner = Instance.new("UICorner")
	UICorner.CornerRadius = UDim.new(0.00, 12.00)
	UICorner.Parent = Template

	local Timer = Instance.new("Frame")
	Timer.Name = "Timer"
	Timer.Size = UDim2.new(1.00, 0.00, 0.00, 2.00)
	Timer.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Timer.Position = UDim2.new(0.00, 0.00, 1.00, -2.00)
	Timer.BorderSizePixel = 0
	Timer.ZIndex = 2
	Timer.BackgroundColor3 = Color3.new(0.43, 0.62, 0.96)
	Timer.Parent = Template

	local Outline = Instance.new("UIStroke")
	Outline.Name = "Outline"
	Outline.Color = Color3.new(0.67, 0.85, 1.40)
	Outline.Thickness = 2
	Outline.Parent = Timer

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.Parent = Timer

	local Scale = Instance.new("UIScale")
	Scale.Name = "Scale"
	Scale.Scale = 0.20000000298023224
	Scale.Parent = Template
	
	-- Scripts:

		local tweenService = game:GetService("TweenService")

		function animateFrame(scale, frame_uiScale)
			tweenService:Create(frame_uiScale, TweenInfo.new(0.25, Enum.EasingStyle.Sine), {
				Scale = scale
			}):Play()
		end

		Close.MouseButton1Up:Connect(function()
			animateFrame(0, CanvasGroup:WaitForChild('UIScale'))
			task.wait(0.3)
			PoltergeistKeySystem:Destroy()

		local tweenService = game:GetService("TweenService")
		local loginInProgress = false -- Variável para evitar múltiplos cliques
		end)
		-- Função para animar o scale da UI
		local function scale(scale, frame_uiScale)
			tweenService:Create(frame_uiScale, TweenInfo.new(0.25, Enum.EasingStyle.Sine), {
				Scale = scale
			}):Play()
		end

		-- Função para exibir notificações
		local function showNotification(title, message, duration)
			local template = Template:Clone()
			template.Parent = Notifications
			template.Frame.Title.Text = title
			template.Frame.Description.Text = message
			scale(1, template:WaitForChild("Scale"))

			-- Barra de progresso
			template.Timer:TweenSize(UDim2.new(0, 0, 0, 2), Enum.EasingDirection.In, Enum.EasingStyle.Sine, duration, true)

			-- Aguarda o tempo da notificação e a remove
			task.delay(duration, function()
				scale(0.2, template:WaitForChild("Scale"))
				task.wait(0.24)
				template:Destroy()
			end)
		end

		-- Lista de usuários e senhas
		local Users = {
			["bernx"] = {
				password = "lobinho10",
				hasKey = true
			},
			["nikhdd1"] = {
				password = "lobinho11",
				hasKey = false
			},
		}

		-- Lista de chaves manualmente definidas e longas
		local Keys = {
			["sdjoWasdAVZS321aasdjzxASVBYU4r23tc"] = {
				assignedAccount = "bernx"
			},
			["GvbsdfjVXNGR23456erTTw234lkjsdk7f8"] = {
				assignedAccount = "nikhdd1"
			}
		}

		local loggedInUser = nil -- Armazena o usuário logado

		Login.Login.MouseButton1Up:Connect(function()
			if loginInProgress then return end -- Impede múltiplos cliques
			loginInProgress = true

			local username = Login.AccountName.TextBox.Text
			local password = Login.AccountPassword.TextBox.Text

			if username ~= "" and password ~= "" then
				if Users[username] then
					if Users[username].password == password then
						loggedInUser = username
						showNotification("Success", "Login successful!", 2)
						task.wait(1)
						Login.Visible = false
						Key.Visible = true
						Key.Title.Text = 'WELCOME BACK, ' .. username

						-- Removendo o Key Mode e atualizando o Key Status
						Navigation.KeyStatus.Text = 'Key Status: VALID'
						-- Alterando a cor para verde (para indicar que está válido)
						Navigation.KeyStatus.TextColor3 = Color3.fromRGB(0, 255, 0)

						-- Verificando se o usuário tem chave
						if Users[username].hasKey then
							Key.Key.Visible = false
							Key.UseKey.Visible = false
						else
							Navigation.KeyStatus.Text = 'Key Status: EXPIRED'
							-- Alterando a cor para vermelho (para indicar que está expirado)
							Navigation.KeyStatus.TextColor3 = Color3.fromRGB(255, 0, 0)
						end
						Navigation:TweenSize(UDim2.new(1, 0, 0.113, 0), Enum.EasingDirection.In, Enum.EasingStyle.Sine, 0.4)
					else
						showNotification("Error", "Incorrect password.", 2)
					end
				else
					showNotification("Error", "Username does not exist.", 2)
				end
			else
				showNotification("Error", "Please fill in all fields.", 2)
			end

			task.wait(1.5) -- Tempo mínimo para evitar spam
			loginInProgress = false
		end)

		Key.UseKey.MouseButton1Up:Connect(function()
			if not loggedInUser then
				showNotification("Error", "You must be logged in to activate a key.", 2)
				return
			end

			local key = Key.Key.TextBox.Text

			if Keys[key] then
				-- Verifica se a chave corresponde à conta do usuário
				if Keys[key].assignedAccount == loggedInUser then
					Users[loggedInUser].hasKey = true
					showNotification("Success", "Key activated successfully!", 2)
					Key.Key.Visible = false
					Key.UseKey.Visible = false
					Navigation.KeyStatus.Text = 'Key Status: VALID'
					-- Alterando a cor para verde (para indicar que está válido)
					Navigation.KeyStatus.TextColor3 = Color3.fromRGB(0, 255, 0)
				else
					showNotification("Error", "This key is not assigned to your account.", 2)
				end
			else
				showNotification("Error", "Invalid key.", 2)
			end
		end)

		Navigation.MainLoader.MouseButton1Up:Connect(function()
			if not loggedInUser or not Users[loggedInUser].hasKey then
				showNotification("Error", "You need a valid key to proceed.", 2)
				return
			end

			-- Oculta a GUI com animação
			scale(0.2, CanvasGroup:FindFirstChild("Scale"))
			task.wait(0.3) -- Pequena espera para a animação terminar

			-- Remove a GUI da memória
			PoltergeistKeySystem:Destroy()

			-- Carrega e executa o MainLoader
			local success, response = pcall(function()
				return loadstring(game:HttpGet("https://raw.githubusercontent.com/berhddb/PoltergeistHub-Mainloader/refs/heads/main/Mainloader"))()
			end)

			-- Caso haja erro ao carregar o script
			if not success then
				warn("Failed to load MainLoader: " .. tostring(response))
				showNotification("Error", "Failed to load MainLoader.", 3)
			end
		end)


	return tab
end

return Library
