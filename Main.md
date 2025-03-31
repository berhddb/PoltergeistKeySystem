-- Código salvo em uma URL ou pastebin
local Library = {}

-- Função para criar sistema de key
function Library:CreateKeySystem()
	local PoltergeistKeySystem = Instance.new("ScreenGui")
	PoltergeistKeySystem.Name = "PoltergeistKeySystem"
	PoltergeistKeySystem.Enabled = false
	PoltergeistKeySystem.ResetOnSpawn = false
	PoltergeistKeySystem.IgnoreGuiInset = true
	PoltergeistKeySystem.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	PoltergeistKeySystem.ScreenInsets = Enum.ScreenInsets.DeviceSafeInsets
	PoltergeistKeySystem.Parent = game:GetService("StarterGui")

	local Notifications = Instance.new("Frame")
	Notifications.Name = "Notifications"
	Notifications.Size = UDim2.new(0.16, 0.00, 0.98, 0.00)
	Notifications.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Notifications.Position = UDim2.new(0.84, 0.00, 0.00, 0.00)
	Notifications.BorderSizePixel = 0
	Notifications.BackgroundTransparency = 1
	Notifications.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Notifications.Parent = PoltergeistKeySystem

	local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint.AspectRatio = 0.3562822639942169
	UIAspectRatioConstraint.Parent = Notifications

	local UIListLayout = Instance.new("UIListLayout")
	UIListLayout.VerticalAlignment = Enum.VerticalAlignment.Bottom
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout.Parent = Notifications

	local CanvasGroup = Instance.new("CanvasGroup")
	CanvasGroup.BorderSizePixel = 0
	CanvasGroup.BackgroundColor3 = Color3.new(0.11, 0.11, 0.11)
	CanvasGroup.AnchorPoint = Vector2.new(0.50, 0.50)
	CanvasGroup.Size = UDim2.new(0.56, 0.00, 0.78, 0.00)
	CanvasGroup.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	CanvasGroup.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	CanvasGroup.Parent = PoltergeistKeySystem

	local Topbar = Instance.new("Frame")
	Topbar.Name = "Topbar"
	Topbar.Size = UDim2.new(1.00, 0.00, 0.11, 0.00)
	Topbar.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Topbar.Position = UDim2.new(0.00, 0.00, 0.00, 0.00)
	Topbar.BorderSizePixel = 0
	Topbar.ZIndex = 2
	Topbar.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Topbar.Parent = CanvasGroup

	local Title = Instance.new("TextLabel")
	Title.Name = "Title"
	Title.TextWrapped = true
	Title.BorderSizePixel = 0
	Title.TextScaled = true
	Title.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title.TextTransparency = 0.5
	Title.AnchorPoint = Vector2.new(0.00, 0.50)
	Title.TextXAlignment = Enum.TextXAlignment.Left
	Title.TextSize = 14
	Title.Size = UDim2.new(0.40, 0.00, 0.38, 0.00)
	Title.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title.Text = "POLTERGEIST KEY SYSTEM"
	Title.TextColor3 = Color3.new(0.39, 0.65, 0.94)
	Title.BackgroundTransparency = 1
	Title.Position = UDim2.new(0.00, 0.00, 0.50, 0.00)
	Title.Parent = Topbar

	local Padding = Instance.new("UIPadding")
	Padding.Name = "Padding"
	Padding.PaddingLeft = UDim.new(0.10, 0.00)
	Padding.Parent = Title

	local TextSize = Instance.new("UITextSizeConstraint")
	TextSize.Name = "TextSize"
	TextSize.MaxTextSize = 30
	TextSize.Parent = Title

	local Close = Instance.new("TextButton")
	Close.Name = "Close"
	Close.BorderSizePixel = 0
	Close.AutoButtonColor = false
	Close.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Close.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Close.AnchorPoint = Vector2.new(0.50, 0.50)
	Close.TextSize = 14
	Close.Size = UDim2.new(0.60, 0.00, 0.60, 0.00)
	Close.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Close.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Close.Text = ""
	Close.BackgroundTransparency = 0.8500000238418579
	Close.Position = UDim2.new(0.97, -10.00, 0.50, 0.00)
	Close.Parent = Topbar

	local Ratio = Instance.new("UIAspectRatioConstraint")
	Ratio.Name = "Ratio"
	Ratio.Parent = Close

	local Corner = Instance.new("UICorner")
	Corner.Name = "Corner"
	Corner.CornerRadius = UDim.new(1.00, 0.00)
	Corner.Parent = Close

	local Icon = Instance.new("ImageLabel")
	Icon.Name = "Icon"
	Icon.ImageColor3 = Color3.new(0.00, 0.00, 0.00)
	Icon.BorderSizePixel = 0
	Icon.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Icon.ImageTransparency = 0.699999988079071
	Icon.AnchorPoint = Vector2.new(0.50, 0.50)
	Icon.Image = "rbxassetid://130426375254962"
	Icon.Size = UDim2.new(0.60, 0.00, 0.60, 0.00)
	Icon.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Icon.BackgroundTransparency = 1
	Icon.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Icon.Parent = Close

	local Constraint = Instance.new("UISizeConstraint")
	Constraint.Name = "Constraint"
	Constraint.MaxSize = Vector2.new(35.00, 35.00)
	Constraint.Parent = Close

	local Scale = Instance.new("UIScale")
	Scale.Name = "Scale"
	Scale.Parent = Close

	local Stroke = Instance.new("UIStroke")
	Stroke.Name = "Stroke"
	Stroke.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
	Stroke.Color = Color3.new(0.41, 0.67, 0.97)
	Stroke.Thickness = 2
	Stroke.Transparency = 0.9599999785423279
	Stroke.Parent = Close

	local LocalScript = Instance.new("LocalScript")
	LocalScript.Source = "local tweenService = game:GetService(\'TweenService\')\n\nfunction animateFrame(scale, frame_uiScale)\n	tweenService:Create(frame_uiScale, TweenInfo.new(0.25, Enum.EasingStyle.Sine), {\n		Scale = scale\n	}):Play()\nend\n\n\n\n\nscript.Parent.MouseButton1Up:Connect(function()\n	animateFrame(0, script.Parent.Parent.Parent:WaitForChild('UIScale'))\n	task.wait(0.3)\n	script.Parent.Parent.Parent.Parent:Destroy()\nend)"
	LocalScript.Parent = Close

	local Stroke_1 = Instance.new("UIStroke")
	Stroke_1.Name = "Stroke"
	Stroke_1.Color = Color3.new(0.38, 0.38, 0.38)
	Stroke_1.Thickness = 2
	Stroke_1.Parent = Topbar

	local Stroke_1 = Instance.new("UIStroke")
	Stroke_1.Name = "Stroke"
	Stroke_1.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
	Stroke_1.Color = Color3.new(0.38, 0.38, 0.38)
	Stroke_1.Thickness = 2.700000047683716
	Stroke_1.Parent = CanvasGroup

	local Corner_1 = Instance.new("UICorner")
	Corner_1.Name = "Corner"
	Corner_1.CornerRadius = UDim.new(0.04, 0.00)
	Corner_1.Parent = CanvasGroup

	local Constraint_1 = Instance.new("UISizeConstraint")
	Constraint_1.Name = "Constraint"
	Constraint_1.MinSize = Vector2.new(250.00, 250.00)
	Constraint_1.Parent = CanvasGroup

	local Ratio_1 = Instance.new("UIAspectRatioConstraint")
	Ratio_1.Name = "Ratio"
	Ratio_1.AspectRatio = 1.350000023841858
	Ratio_1.Parent = CanvasGroup

	local Dots = Instance.new("ImageLabel")
	Dots.Name = "Dots"
	Dots.BorderSizePixel = 0
	Dots.ScaleType = Enum.ScaleType.Tile
	Dots.BackgroundColor3 = Color3.new(0.12, 0.12, 0.12)
	Dots.ImageTransparency = 0.8999999761581421
	Dots.Image = "rbxassetid://6803353442"
	Dots.TileSize = UDim2.new(0.00, 30.00, 0.00, 30.00)
	Dots.Size = UDim2.new(1.21, 0.00, 1.62, 0.00)
	Dots.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Dots.Rotation = 45
	Dots.BackgroundTransparency = 1
	Dots.Position = UDim2.new(-0.10, 0.00, -0.31, 0.00)
	Dots.Parent = CanvasGroup

	local Key = Instance.new("Frame")
	Key.Name = "Key"
	Key.Visible = false
	Key.Size = UDim2.new(0.00, 623.00, 0.00, 361.00)
	Key.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Key.Position = UDim2.new(0.00, 0.00, 0.11, 0.00)
	Key.BorderSizePixel = 0
	Key.BackgroundTransparency = 1
	Key.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Key.Parent = CanvasGroup

	local Title_1 = Instance.new("TextLabel")
	Title_1.Name = "Title"
	Title_1.TextWrapped = true
	Title_1.BorderSizePixel = 0
	Title_1.TextScaled = true
	Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title_1.TextTransparency = 0.5
	Title_1.AnchorPoint = Vector2.new(0.00, 0.50)
	Title_1.TextXAlignment = Enum.TextXAlignment.Left
	Title_1.TextSize = 14
	Title_1.Size = UDim2.new(0.45, 0.00, 0.18, 0.00)
	Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title_1.Text = "WELCOME BACK, PLAYER!"
	Title_1.TextColor3 = Color3.new(0.39, 0.65, 0.94)
	Title_1.BackgroundTransparency = 1
	Title_1.Position = UDim2.new(-0.01, 0.00, 0.11, 0.00)
	Title_1.Parent = Key

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = Title_1

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = Title_1

	local Key_1 = Instance.new("Frame")
	Key_1.Name = "Key"
	Key_1.Size = UDim2.new(0.30, 0.00, 0.12, 0.00)
	Key_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Key_1.Position = UDim2.new(0.03, 0.00, 0.24, 0.00)
	Key_1.BorderSizePixel = 0
	Key_1.BackgroundColor3 = Color3.new(0.17, 0.17, 0.17)
	Key_1.Parent = Key

	local UIStroke = Instance.new("UIStroke")
	UIStroke.Color = Color3.new(0.46, 0.46, 0.46)
	UIStroke.Parent = Key_1

	local UICorner = Instance.new("UICorner")
	UICorner.CornerRadius = UDim.new(0.00, 16.00)
	UICorner.Parent = Key_1

	local TextBox = Instance.new("TextBox")
	TextBox.BorderSizePixel = 0
	TextBox.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox.TextSize = 14
	TextBox.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	TextBox.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox.Text = ""
	TextBox.TextXAlignment = Enum.TextXAlignment.Left
	TextBox.BackgroundTransparency = 1
	TextBox.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox.Parent = Key_1

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.708333492279053
	UIAspectRatioConstraint_1.Parent = TextBox

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = Key_1

	local Asterisco = Instance.new("TextLabel")
	Asterisco.Name = "Asterisco"
	Asterisco.TextWrapped = true
	Asterisco.ZIndex = 3
	Asterisco.BorderSizePixel = 0
	Asterisco.TextScaled = true
	Asterisco.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Asterisco.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Asterisco.TextTransparency = 0.5
	Asterisco.AnchorPoint = Vector2.new(0.00, 0.50)
	Asterisco.TextSize = 100
	Asterisco.Size = UDim2.new(0.11, 0.00, 0.44, 0.00)
	Asterisco.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Asterisco.Text = "*"
	Asterisco.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	Asterisco.BackgroundTransparency = 1
	Asterisco.Position = UDim2.new(0.86, 0.00, 0.38, 0.00)
	Asterisco.Parent = Key_1

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = Asterisco

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = Asterisco

	local UseKey = Instance.new("TextButton")
	UseKey.Name = "UseKey"
	UseKey.Active = false
	UseKey.BorderSizePixel = 0
	UseKey.BackgroundColor3 = Color3.new(0.13, 0.90, 0.07)
	UseKey.Size = UDim2.new(0.26, 0.00, 1.22, 0.00)
	UseKey.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	UseKey.Text = ""
	UseKey.Position = UDim2.new(0.03, 0.00, 0.39, 0.00)
	UseKey.Selectable = false
	UseKey.Parent = Key

	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.19, 0.46, 0.02)
	UIStroke_1.Thickness = 1.5
	UIStroke_1.Parent = UseKey

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 16.00)
	UICorner_1.Parent = UseKey

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = UseKey

	local TextBox_1 = Instance.new("TextLabel")
	TextBox_1.Name = "TextBox"
	TextBox_1.TextWrapped = true
	TextBox_1.Active = true
	TextBox_1.BorderSizePixel = 0
	TextBox_1.TextScaled = true
	TextBox_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox_1.TextSize = 14
	TextBox_1.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox_1.Selectable = true
	TextBox_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox_1.Text = "USE KEY"
	TextBox_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.BackgroundTransparency = 1
	TextBox_1.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox_1.Parent = UseKey

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.7083330154418945
	UIAspectRatioConstraint_1.Parent = TextBox_1

	local LoginAndKeySystem = Instance.new("LocalScript")
	LoginAndKeySystem.Name = "LoginAndKeySystem"
	LoginAndKeySystem.Source = "local tweenService = game:GetService(\'TweenService\')\nlocal loginInProgress = false -- Variável para evitar múltiplos cliques\n\n-- Função para animar o scale da UI\nlocal function scale(scale, frame_uiScale)\n	tweenService:Create(frame_uiScale, TweenInfo.new(0.25, Enum.EasingStyle.Sine), {\n		Scale = scale\n	}):Play()\nend\n\n-- Função para exibir notificações\nlocal function showNotification(title, message, duration)\n	local template = script.Template:Clone()\n	template.Parent = script.Parent.Parent.Notifications\n	template.Frame.Title.Text = title\n	template.Frame.Description.Text = message\n	scale(1, template:WaitForChild(\'Scale\'))\n\n	-- Barra de progresso\n	template.Timer:TweenSize(UDim2.new(0, 0, 0, 2), Enum.EasingDirection.In, Enum.EasingStyle.Sine, duration, true)\n\n	-- Aguarda o tempo da notificação e a remove\n	task.delay(duration, function()\n		scale(0.2, template:WaitForChild(\'Scale\'))\n		task.wait(0.24)\n		template:Destroy()\n	end)\nend\n\n-- Lista de usuários e senhas\nlocal Users = {\n	[\'bernx\'] = {\n		password = \'lobinho10\',\n		hasKey = true\n	},\n	[\'nikhdd1\'] = {\n		password = \'lobinho11\',\n		hasKey = false\n	},\n}\n\n-- Lista de chaves manualmente definidas e longas\nlocal Keys = {\n	[\'sdjoWasdAVZS321aasdjzxASVBYU4r23tc\'] = {\n		assignedAccount = \'bernx\'\n	},\n	[\'GvbsdfjVXNGR23456erTTw234lkjsdk7f8\'] = {\n		assignedAccount = \'nikhdd1\'\n	}\n}\n\nlocal loggedInUser = nil -- Armazena o usuário logado\n\nscript.Parent.Login.Login.MouseButton1Up:Connect(function()\n	if loginInProgress then return end -- Impede múltiplos cliques\n	loginInProgress = true\n\n	local username = script.Parent.Login.AccountName.TextBox.Text\n	local password = script.Parent.Login.AccountPassword.TextBox.Text\n\n	if username ~= \'\' and password ~= \'\' then\n		if Users[username] then\n			if Users[username].password == password then\n				loggedInUser = username\n				showNotification(\'Success\', \'Login successful!\', 2)\n				task.wait(1)\n				script.Parent.Login.Visible = false\n				script.Parent.Key.Visible = true\n				script.Parent.Key.Title.Text = 'WELCOME BACK, ' .. username\n\n				-- Removendo o Key Mode e atualizando o Key Status\n				script.Parent.Navigation.KeyStatus.Text = 'Key Status: VALID'\n				-- Alterando a cor para verde (para indicar que está válido)\n				script.Parent.Navigation.KeyStatus.TextColor3 = Color3.fromRGB(0, 255, 0)\n\n				-- Verificando se o usuário tem chave\n				if Users[username].hasKey then\n					script.Parent.Key.Key.Visible = false\n					script.Parent.Key.UseKey.Visible = false\n				else\n					script.Parent.Navigation.KeyStatus.Text = 'Key Status: EXPIRED'\n					-- Alterando a cor para vermelho (para indicar que está expirado)\n					script.Parent.Navigation.KeyStatus.TextColor3 = Color3.fromRGB(255, 0, 0)\n				end\n				script.Parent.Navigation:TweenSize(UDim2.new(1, 0, 0.113, 0), Enum.EasingDirection.In, Enum.EasingStyle.Sine, 0.4)\n			else\n				showNotification(\'Error\', \'Incorrect password.\', 2)\n			end\n		else\n			showNotification(\'Error\', \'Username does not exist.\', 2)\n		end\n	else\n		showNotification(\'Error\', \'Please fill in all fields.\', 2)\n	end\n\n	task.wait(1.5) -- Tempo mínimo para evitar spam\n	loginInProgress = false\nend)\n\nscript.Parent.Key.UseKey.MouseButton1Up:Connect(function()\n	if not loggedInUser then\n		showNotification(\'Error\', \'You must be logged in to activate a key.\', 2)\n		return\n	end\n\n	local key = script.Parent.Key.Key.TextBox.Text\n\n	if Keys[key] then\n		-- Verifica se a chave corresponde à conta do usuário\n		if Keys[key].assignedAccount == loggedInUser then\n			Users[loggedInUser].hasKey = true\n			showNotification(\'Success\', \'Key activated successfully!\', 2)\n			script.Parent.Key.Key.Visible = false\n			script.Parent.Key.UseKey.Visible = false\n			script.Parent.Navigation.KeyStatus.Text = 'Key Status: VALID'\n			-- Alterando a cor para verde (para indicar que está válido)\n			script.Parent.Navigation.KeyStatus.TextColor3 = Color3.fromRGB(0, 255, 0)\n		else\n			showNotification(\'Error\', \'This key is not assigned to your account.\', 2)\n		end\n	else\n		showNotification(\'Error\', \'Invalid key.\', 2)\n	end\nend)\n\nscript.Parent.Navigation.MainLoader.MouseButton1Up:Connect(function()\n	if not loggedInUser or not Users[loggedInUser].hasKey then\n		showNotification(\'Error\', \'You need a valid key to proceed.\', 2)\n		return\n	end\n\n	-- Oculta a GUI com animação\n	scale(0.2, script.Parent:FindFirstChild(\'Scale\'))\n	task.wait(0.3) -- Pequena espera para a animação terminar\n\n	-- Remove a GUI da memória\n	script.Parent:Destroy()\n\n	-- Carrega e executa o MainLoader\n	local success, response = pcall(function()\n		return loadstring(game:HttpGet(\'https://raw.githubusercontent.com/berhddb/PoltergeistHub-Mainloader/refs/heads/main/Mainloader\'))()\n	end)\n\n	-- Caso haja erro ao carregar o script\n	if not success then\n		warn(\'Failed to load MainLoader: \' .. tostring(response))\n		showNotification(\'Error\', \'Failed to load MainLoader.\', 3)\n	end\nend)\n"
	LoginAndKeySystem.Parent = CanvasGroup

	local Template = Instance.new("CanvasGroup")
	Template.Name = "Template"
	Template.BorderSizePixel = 0
	Template.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Template.AutomaticSize = Enum.AutomaticSize.Y
	Template.Size = UDim2.new(0.96, 0.00, 0.13, 0.00)
	Template.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Template.Position = UDim2.new(1.00, 0.00, 1.00, 0.00)
	Template.Parent = LoginAndKeySystem

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

	local UIListLayout_1 = Instance.new("UIListLayout")
	UIListLayout_1.VerticalAlignment = Enum.VerticalAlignment.Center
	UIListLayout_1.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout_1.Parent = Frame

	local Title_1 = Instance.new("TextLabel")
	Title_1.Name = "Title"
	Title_1.TextWrapped = true
	Title_1.ZIndex = 2
	Title_1.BorderSizePixel = 0
	Title_1.RichText = true
	Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title_1.AnchorPoint = Vector2.new(0.50, 0.00)
	Title_1.TextXAlignment = Enum.TextXAlignment.Left
	Title_1.TextSize = 16
	Title_1.Size = UDim2.new(1.00, 0.00, 0.00, 10.00)
	Title_1.Text = "Title"
	Title_1.TextColor3 = Color3.new(0.41, 0.41, 0.41)
	Title_1.AutomaticSize = Enum.AutomaticSize.Y
	Title_1.BackgroundTransparency = 1
	Title_1.Position = UDim2.new(0.50, 0.00, -0.52, 15.00)
	Title_1.Parent = Frame

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

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 12.00)
	UICorner_1.Parent = Template

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

	local Scale_1 = Instance.new("UIScale")
	Scale_1.Name = "Scale"
	Scale_1.Scale = 0.20000000298023224
	Scale_1.Parent = Template

	local Login = Instance.new("Frame")
	Login.Name = "Login"
	Login.Size = UDim2.new(0.00, 623.00, 0.00, 361.00)
	Login.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Login.Position = UDim2.new(0.00, 0.00, 0.11, 0.00)
	Login.BorderSizePixel = 0
	Login.BackgroundTransparency = 1
	Login.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Login.Parent = CanvasGroup

	local Title_1 = Instance.new("TextLabel")
	Title_1.Name = "Title"
	Title_1.TextWrapped = true
	Title_1.BorderSizePixel = 0
	Title_1.TextScaled = true
	Title_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title_1.TextTransparency = 0.5
	Title_1.AnchorPoint = Vector2.new(0.00, 0.50)
	Title_1.TextXAlignment = Enum.TextXAlignment.Left
	Title_1.TextSize = 14
	Title_1.Size = UDim2.new(0.45, 0.00, 0.18, 0.00)
	Title_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title_1.Text = "LOGIN POLTERGEIST HUB"
	Title_1.TextColor3 = Color3.new(0.39, 0.65, 0.94)
	Title_1.BackgroundTransparency = 1
	Title_1.Position = UDim2.new(-0.01, 0.00, 0.11, 0.00)
	Title_1.Parent = Login

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = Title_1

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = Title_1

	local AccountName = Instance.new("Frame")
	AccountName.Name = "AccountName"
	AccountName.Size = UDim2.new(0.30, 0.00, 0.12, 0.00)
	AccountName.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	AccountName.Position = UDim2.new(0.04, 0.00, 0.40, 0.00)
	AccountName.BorderSizePixel = 0
	AccountName.BackgroundColor3 = Color3.new(0.17, 0.17, 0.17)
	AccountName.Parent = Login

	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.46, 0.46, 0.46)
	UIStroke_1.Parent = AccountName

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 16.00)
	UICorner_1.Parent = AccountName

	local TextBox_1 = Instance.new("TextBox")
	TextBox_1.BorderSizePixel = 0
	TextBox_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox_1.TextSize = 14
	TextBox_1.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox_1.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	TextBox_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox_1.Text = ""
	TextBox_1.TextXAlignment = Enum.TextXAlignment.Left
	TextBox_1.BackgroundTransparency = 1
	TextBox_1.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox_1.Parent = AccountName

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.708333492279053
	UIAspectRatioConstraint_1.Parent = TextBox_1

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = AccountName

	local Asterisco_1 = Instance.new("TextLabel")
	Asterisco_1.Name = "Asterisco"
	Asterisco_1.TextWrapped = true
	Asterisco_1.ZIndex = 3
	Asterisco_1.BorderSizePixel = 0
	Asterisco_1.TextScaled = true
	Asterisco_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Asterisco_1.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Asterisco_1.TextTransparency = 0.5
	Asterisco_1.AnchorPoint = Vector2.new(0.00, 0.50)
	Asterisco_1.TextSize = 100
	Asterisco_1.Size = UDim2.new(0.11, 0.00, 0.44, 0.00)
	Asterisco_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Asterisco_1.Text = "*"
	Asterisco_1.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	Asterisco_1.BackgroundTransparency = 1
	Asterisco_1.Position = UDim2.new(0.86, 0.00, 0.38, 0.00)
	Asterisco_1.Parent = AccountName

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = Asterisco_1

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = Asterisco_1

	local AccountPassword = Instance.new("Frame")
	AccountPassword.Name = "AccountPassword"
	AccountPassword.Size = UDim2.new(0.30, 0.00, 0.12, 0.00)
	AccountPassword.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	AccountPassword.Position = UDim2.new(0.04, 0.00, 0.54, 0.00)
	AccountPassword.BorderSizePixel = 0
	AccountPassword.BackgroundColor3 = Color3.new(0.17, 0.17, 0.17)
	AccountPassword.Parent = Login

	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.46, 0.46, 0.46)
	UIStroke_1.Parent = AccountPassword

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 16.00)
	UICorner_1.Parent = AccountPassword

	local TextBox_1 = Instance.new("TextBox")
	TextBox_1.BorderSizePixel = 0
	TextBox_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox_1.TextSize = 14
	TextBox_1.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox_1.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	TextBox_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox_1.Text = ""
	TextBox_1.TextXAlignment = Enum.TextXAlignment.Left
	TextBox_1.BackgroundTransparency = 1
	TextBox_1.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox_1.Parent = AccountPassword

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.7083330154418945
	UIAspectRatioConstraint_1.Parent = TextBox_1

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = AccountPassword

	local Asterisco_1 = Instance.new("TextLabel")
	Asterisco_1.Name = "Asterisco"
	Asterisco_1.TextWrapped = true
	Asterisco_1.ZIndex = 3
	Asterisco_1.BorderSizePixel = 0
	Asterisco_1.TextScaled = true
	Asterisco_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Asterisco_1.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Asterisco_1.TextTransparency = 0.5
	Asterisco_1.AnchorPoint = Vector2.new(0.00, 0.50)
	Asterisco_1.TextSize = 100
	Asterisco_1.Size = UDim2.new(0.11, 0.00, 0.44, 0.00)
	Asterisco_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Asterisco_1.Text = "*"
	Asterisco_1.TextColor3 = Color3.new(0.52, 0.52, 0.52)
	Asterisco_1.BackgroundTransparency = 1
	Asterisco_1.Position = UDim2.new(0.86, 0.00, 0.38, 0.00)
	Asterisco_1.Parent = AccountPassword

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = Asterisco_1

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = Asterisco_1

	local Login_1 = Instance.new("TextButton")
	Login_1.Name = "Login"
	Login_1.Active = false
	Login_1.BorderSizePixel = 0
	Login_1.BackgroundColor3 = Color3.new(0.13, 0.90, 0.07)
	Login_1.Size = UDim2.new(0.25, 0.00, 0.11, 0.00)
	Login_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Login_1.Text = ""
	Login_1.Position = UDim2.new(0.06, 0.00, 0.68, 0.00)
	Login_1.Selectable = false
	Login_1.Parent = Login

	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.19, 0.46, 0.02)
	UIStroke_1.Thickness = 1.5
	UIStroke_1.Parent = Login_1

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 16.00)
	UICorner_1.Parent = Login_1

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = Login_1

	local TextBox_1 = Instance.new("TextLabel")
	TextBox_1.Name = "TextBox"
	TextBox_1.TextWrapped = true
	TextBox_1.Active = true
	TextBox_1.BorderSizePixel = 0
	TextBox_1.TextScaled = true
	TextBox_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox_1.TextSize = 14
	TextBox_1.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox_1.Selectable = true
	TextBox_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox_1.Text = "Log in"
	TextBox_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.BackgroundTransparency = 1
	TextBox_1.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox_1.Parent = Login_1

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.7083330154418945
	UIAspectRatioConstraint_1.Parent = TextBox_1

	local Navigation = Instance.new("Frame")
	Navigation.Name = "Navigation"
	Navigation.Active = true
	Navigation.AnchorPoint = Vector2.new(0.00, 1.00)
	Navigation.Size = UDim2.new(1.00, 0.00, 0.00, 0.00)
	Navigation.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Navigation.Position = UDim2.new(0.00, 0.00, 1.00, 0.00)
	Navigation.BorderSizePixel = 0
	Navigation.ZIndex = 2
	Navigation.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Navigation.Parent = CanvasGroup

	local Outline_1 = Instance.new("UIStroke")
	Outline_1.Name = "Outline"
	Outline_1.Transparency = 0.9700000286102295
	Outline_1.Parent = Navigation

	local Stroke_1 = Instance.new("UIStroke")
	Stroke_1.Name = "Stroke"
	Stroke_1.Color = Color3.new(0.38, 0.38, 0.38)
	Stroke_1.Thickness = 2
	Stroke_1.Parent = Navigation

	local MainLoader = Instance.new("TextButton")
	MainLoader.Name = "MainLoader"
	MainLoader.Active = false
	MainLoader.BorderSizePixel = 0
	MainLoader.BackgroundColor3 = Color3.new(0.13, 0.90, 0.07)
	MainLoader.Size = UDim2.new(0.26, 0.00, 1.22, 0.00)
	MainLoader.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	MainLoader.Text = ""
	MainLoader.Position = UDim2.new(0.03, 0.00, 0.13, 0.00)
	MainLoader.Selectable = false
	MainLoader.Parent = Navigation

	local UIStroke_1 = Instance.new("UIStroke")
	UIStroke_1.Color = Color3.new(0.19, 0.46, 0.02)
	UIStroke_1.Thickness = 1.5
	UIStroke_1.Parent = MainLoader

	local UICorner_1 = Instance.new("UICorner")
	UICorner_1.CornerRadius = UDim.new(0.00, 16.00)
	UICorner_1.Parent = MainLoader

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 4.452381134033203
	UIAspectRatioConstraint_1.Parent = MainLoader

	local TextBox_1 = Instance.new("TextLabel")
	TextBox_1.Name = "TextBox"
	TextBox_1.TextWrapped = true
	TextBox_1.Active = true
	TextBox_1.BorderSizePixel = 0
	TextBox_1.TextScaled = true
	TextBox_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	TextBox_1.TextSize = 14
	TextBox_1.Size = UDim2.new(0.86, 0.00, 0.57, 0.00)
	TextBox_1.Selectable = true
	TextBox_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	TextBox_1.Text = "OPEN HUB"
	TextBox_1.TextColor3 = Color3.new(1.00, 1.00, 1.00)
	TextBox_1.BackgroundTransparency = 1
	TextBox_1.Position = UDim2.new(0.07, 0.00, 0.21, 0.00)
	TextBox_1.Parent = MainLoader

	local UIAspectRatioConstraint_1 = Instance.new("UIAspectRatioConstraint")
	UIAspectRatioConstraint_1.AspectRatio = 6.7083330154418945
	UIAspectRatioConstraint_1.Parent = TextBox_1

	local KeyStatus = Instance.new("TextLabel")
	KeyStatus.Name = "KeyStatus"
	KeyStatus.TextWrapped = true
	KeyStatus.BorderSizePixel = 0
	KeyStatus.TextScaled = true
	KeyStatus.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	KeyStatus.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	KeyStatus.TextTransparency = 0.5
	KeyStatus.AnchorPoint = Vector2.new(0.00, 0.50)
	KeyStatus.TextXAlignment = Enum.TextXAlignment.Right
	KeyStatus.TextSize = 14
	KeyStatus.Size = UDim2.new(0.30, 0.00, 0.31, 0.00)
	KeyStatus.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	KeyStatus.Text = "KEY STATUS: VALID"
	KeyStatus.TextColor3 = Color3.new(0.49, 0.98, 0.00)
	KeyStatus.BackgroundTransparency = 1
	KeyStatus.Position = UDim2.new(0.67, 0.00, 0.67, 0.00)
	KeyStatus.Parent = Navigation

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingLeft = UDim.new(0.10, 0.00)
	Padding_1.Parent = KeyStatus

	local TextSize_1 = Instance.new("UITextSizeConstraint")
	TextSize_1.Name = "TextSize"
	TextSize_1.MaxTextSize = 30
	TextSize_1.Parent = KeyStatus

	return tab
end

return Library
