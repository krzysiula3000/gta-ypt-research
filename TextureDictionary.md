# Texture Dictionary Properties
**Name** - Unique name used to reference this texture in ParticleRules' ShaderVars section

**Unk32** - 
_(Usually 128 or 32)_

**Usage** - 
_(DIFFUSE, NORMAL, SPEC)_

**UsageFlags**

**ExtraFlags**

**Width** - px

**Height** - px

**MipLevels** - Number of MipMaps, starts from 0

**Format** - Compression format 
_(D3DFMT_DXT1, D3DFMT_DXT5)_

**FileName** - Name of the texture image file


## Example Structure
	<TextureDictionary>
		<Item>
			<Name>_explosion_fireball</Name>
			<Unk32 value="128"/>
			<Usage>DIFFUSE</Usage>
			<UsageFlags>X32, X64, X128, X512, X1024, UNK24</UsageFlags>
			<ExtraFlags value="0"/>
			<Width value="1024"/>
			<Height value="1024"/>
			<MipLevels value="11"/>
			<Format>D3DFMT_DXT1</Format>
			<FileName>_explosion_fireball.dds</FileName>
		</Item>
	</TextureDictionary>
