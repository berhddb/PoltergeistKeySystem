-- Código salvo em uma URL ou pastebin
local Library = {}

-- Função para criar janela
function Library:CreateWindow(options)
	local PoltergeistHub = Instance.new("ScreenGui")
	PoltergeistHub.Name = options.Name or "Window"
	PoltergeistHub.ResetOnSpawn = false
	PoltergeistHub.IgnoreGuiInset = true
	PoltergeistHub.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	PoltergeistHub.ScreenInsets = Enum.ScreenInsets.DeviceSafeInsets
	PoltergeistHub.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

	local CanvasGroup = Instance.new("CanvasGroup")
	CanvasGroup.BorderSizePixel = 0
	CanvasGroup.BackgroundColor3 = Color3.new(0.11, 0.11, 0.11)
	CanvasGroup.AnchorPoint = Vector2.new(0.50, 0.50)
	CanvasGroup.Size = UDim2.new(0.56, 0.00, 0.78, 0.00)
	CanvasGroup.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	CanvasGroup.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	CanvasGroup.Parent = PoltergeistHub

	local Topbar = Instance.new("Frame")
	Topbar.Name = "Topbar"
	Topbar.Size = UDim2.new(1.00, 0.00, 0.11, 0.00)
	Topbar.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Topbar.Position = UDim2.new(0.00, 0.00, 0.00, 0.00)
	Topbar.BorderSizePixel = 0
	Topbar.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Topbar.Parent = CanvasGroup

	local Title = Instance.new("TextLabel")
	Title.Name = "Title"
	Title.TextWrapped = true
	Title.BorderSizePixel = 0
	Title.TextScaled = true
	Title.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Title.FontFace = Font.new("rbxassetid://12187365364", Enum.FontWeight.Bold, Enum.FontStyle.Normal)
	Title.TextTransparency = 0.5
	Title.AnchorPoint = Vector2.new(0.00, 0.50)
	Title.TextXAlignment = Enum.TextXAlignment.Left
	Title.TextSize = 14
	Title.Size = UDim2.new(0.40, 0.00, 0.38, 0.00)
	Title.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Title.Text = "POLTERGEIST HUB"
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
	Close.BackgroundColor3 = Color3.new(0.39, 0.65, 0.94)
	Close.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Close.AnchorPoint = Vector2.new(0.50, 0.50)
	Close.TextSize = 14
	Close.Size = UDim2.new(0.60, 0.00, 0.60, 0.00)
	Close.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Close.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Close.Text = ""
	Close.BackgroundTransparency = 0.949999988079071
	Close.Position = UDim2.new(0.95, -10.00, 0.50, 0.00)
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
	Icon.ImageTransparency = 0.8999999761581421
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

	local Navigation = Instance.new("Frame")
	Navigation.Name = "Navigation"
	Navigation.Active = true
	Navigation.AnchorPoint = Vector2.new(0.00, 1.00)
	Navigation.Size = UDim2.new(1.00, 0.00, 0.11, 0.00)
	Navigation.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Navigation.Position = UDim2.new(0.00, 0.00, 1.00, 0.00)
	Navigation.BorderSizePixel = 0
	Navigation.BackgroundColor3 = Color3.new(0.15, 0.15, 0.15)
	Navigation.Parent = CanvasGroup

	local Outline = Instance.new("UIStroke")
	Outline.Name = "Outline"
	Outline.Transparency = 0.9700000286102295
	Outline.Parent = Navigation

	local Scroller = Instance.new("ScrollingFrame")
	Scroller.Name = "Scroller"
	Scroller.Active = true
	Scroller.BorderSizePixel = 0
	Scroller.CanvasSize = UDim2.new(0.00, 0.00, 0.00, 0.00)
	Scroller.AutomaticCanvasSize = Enum.AutomaticSize.X
	Scroller.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Scroller.Size = UDim2.new(1.00, 0.00, 0.94, 0.00)
	Scroller.ScrollBarImageColor3 = Color3.new(0.00, 0.00, 0.00)
	Scroller.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Scroller.ScrollBarThickness = 5
	Scroller.ScrollBarImageTransparency = 0.800000011920929
	Scroller.BackgroundTransparency = 1
	Scroller.Parent = Navigation

	local Layout = Instance.new("UIListLayout")
	Layout.Name = "Layout"
	Layout.FillDirection = Enum.FillDirection.Horizontal
	Layout.HorizontalAlignment = Enum.HorizontalAlignment.Center
	Layout.VerticalAlignment = Enum.VerticalAlignment.Center
	Layout.Padding = UDim.new(0.05, 0.00)
	Layout.SortOrder = Enum.SortOrder.LayoutOrder
	Layout.Parent = Scroller

	local Padding_1 = Instance.new("UIPadding")
	Padding_1.Name = "Padding"
	Padding_1.PaddingRight = UDim.new(0.00, 10.00)
	Padding_1.Parent = Scroller

	local Template = Instance.new("TextButton")
	Template.Name = "Template"
	Template.Visible = false
	Template.BorderSizePixel = 0
	Template.AutoButtonColor = false
	Template.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Template.FontFace = Font.new("rbxasset://fonts/families/SourceSansPro.json", Enum.FontWeight.Regular, Enum.FontStyle.Normal)
	Template.AnchorPoint = Vector2.new(0.50, 0.50)
	Template.TextSize = 14
	Template.Size = UDim2.new(1.20, 0.00, 0.18, 0.00)
	Template.TextColor3 = Color3.new(0.00, 0.00, 0.00)
	Template.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Template.Text = ""
	Template.Position = UDim2.new(1.45, 0.00, 0.22, 0.00)
	Template.Parent = Scroller

	local Corner_1 = Instance.new("UICorner")
	Corner_1.Name = "Corner"
	Corner_1.CornerRadius = UDim.new(0.00, 9.00)
	Corner_1.Parent = Template

	local Icon_1 = Instance.new("ImageLabel")
	Icon_1.Name = "Icon"
	Icon_1.ImageColor3 = Color3.new(0.92, 0.76, 0.76)
	Icon_1.BorderSizePixel = 0
	Icon_1.BackgroundColor3 = Color3.new(1.00, 1.00, 1.00)
	Icon_1.ImageTransparency = 0.20000000298023224
	Icon_1.AnchorPoint = Vector2.new(0.50, 0.50)
	Icon_1.Image = "http://www.roblox.com/asset/?id=6026568201"
	Icon_1.Size = UDim2.new(0.61, 0.00, 0.61, 0.00)
	Icon_1.BorderColor3 = Color3.new(0.00, 0.00, 0.00)
	Icon_1.BackgroundTransparency = 1
	Icon_1.Position = UDim2.new(0.50, 0.00, 0.50, 0.00)
	Icon_1.Parent = Template

	local Stroke_1 = Instance.new("UIStroke")
	Stroke_1.Name = "Stroke"
	Stroke_1.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
	Stroke_1.Color = Color3.new(0.16, 0.14, 0.14)
	Stroke_1.Thickness = 1.5
	Stroke_1.Transparency = 0.8999999761581421
	Stroke_1.Parent = Template

	local Ratio_1 = Instance.new("UIAspectRatioConstraint")
	Ratio_1.Name = "Ratio"
	Ratio_1.AspectRatio = 0.976239800453186
	Ratio_1.Parent = Template

	local Scale_1 = Instance.new("UIScale")
	Scale_1.Name = "Scale"
	Scale_1.Parent = Template

	local Gradient = Instance.new("UIGradient")
	Gradient.Name = "Gradient"
	Gradient.Transparency = NumberSequence.new(NumberSequenceKeypoint.new(0.00, 0.05, 0.00), NumberSequenceKeypoint.new(1.00, 0.05, 0.00))
	Gradient.Color = ColorSequence.new(ColorSequenceKeypoint.new(0.00, Color3.new(1.00, 1.00, 1.00)), ColorSequenceKeypoint.new(1.00, Color3.new(0.95, 0.78, 0.78)))
	Gradient.Offset = Vector2.new(0.00, 0.58)
	Gradient.Rotation = 70
	Gradient.Parent = Template

	local Constraint_1 = Instance.new("UISizeConstraint")
	Constraint_1.Name = "Constraint"
	Constraint_1.MinSize = Vector2.new(35.00, 35.00)
	Constraint_1.MaxSize = Vector2.new(70.00, 70.00)
	Constraint_1.Parent = Template

	local Stroke_1 = Instance.new("UIStroke")
	Stroke_1.Name = "Stroke"
	Stroke_1.Color = Color3.new(0.38, 0.38, 0.38)
	Stroke_1.Thickness = 2
	Stroke_1.Parent = Navigation

	local Constraint_1 = Instance.new("UISizeConstraint")
	Constraint_1.Name = "Constraint"
	Constraint_1.MinSize = Vector2.new(250.00, 250.00)
	Constraint_1.Parent = CanvasGroup

	local Ratio_1 = Instance.new("UIAspectRatioConstraint")
	Ratio_1.Name = "Ratio"
	Ratio_1.AspectRatio = 1.350000023841858
	Ratio_1.Parent = CanvasGroup

	local UIDrag = Instance.new("LocalScript")
	UIDrag.Name = "UIDrag"
	UIDrag.Parent = CanvasGroup
	return window
end

-- Função para criar aba
function Library:CreateTab(window, tabName)
	print(tabName)
	return tab
end

return Library
