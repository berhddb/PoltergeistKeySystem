-- Código salvo em uma URL ou pastebin
local Library = {}

-- Função para criar janela
function Library:CreateWindow(options)
    local window = Instance.new("ScreenGui")
    window.Name = options.Name or "Window"
    window.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
    return window
end

-- Função para criar aba
function Library:CreateTab(window, tabName)
    local tab = Instance.new("Frame")
    tab.Name = tabName
    tab.Size = UDim2.new(0, 200, 0, 50)
    tab.Parent = window
    return tab
end

return Library
