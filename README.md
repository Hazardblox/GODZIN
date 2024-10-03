-- Certifique-se de que o jogo está carregado
repeat wait() until game:IsLoaded()

-- Configurações do script
_G.HOHO_autoBounty = {
    TransparencyGui = true,
    AutoTeam = "Pirate", -- Pode ser "Pirate" ou "Marine"
    Webhook = "", -- URL do webhook para notificações (opcional)
    BypassTeleport = false, -- Não usar
    SkipLeopardAndBuddah = false,
    MaxTimeTarget = 120, -- Tempo máximo para atacar um alvo
    ["Dont attack player have Cup"] = false,
    Character_Config = {
        InvisibleCharacter = true, -- Usar um pacote de personagem invisível
        InvisFromKen = true,
        NoStun = true,
    },
    Skill_Config = {
        ["Melee"] = {
            Z = {Enabled = false, Hold = 0.1},
            X = {Enabled = false, Hold = 0.1},
            C = {Enabled = false, Hold = 0.1},
        },
        ["Sword"] = {
            Z = {Enabled = false, Hold = 0.1},
            X = {Enabled = false, Hold = 0.1},
        },
        ["Gun"] = {
            Z = {Enabled = false, Hold = 0.1},
            X = {Enabled = false, Hold = 0.1},
        },
        ["Fruit"] = {
            Z = {Enabled = true, Hold = 0.3},
            X = {Enabled = true, Hold = 0.2},
            C = {Enabled = true, Hold = 0.2},
            V = {Enabled = true, Hold = 0.1},
            F = {Enabled = true, Hold = 0.2},
        },
    },
}

-- Carregar o script principal
loadstring(game:HttpGet('https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI'))()
