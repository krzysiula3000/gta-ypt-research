# Particle Rule Properties
## Header Info
**Name** - Unique Particle Rule name, used to target it in EffectRuleDictionary

**FxcFile** - .fxc shader dictionary name

**FxcTechnique** - Shader technique name

## Header

**Unknown10**

**Unknown100**

**Unknown104** - bit - Enables particle texture alpha (transparency)

**Unknown108**

**Unknown10C** - flag

**Unknown118** - frames? - Min texture animation speed

**Unknown11C** - frames? - Max texture animation speed

**Unknown1D0**

**Unknown1E0**

**Unknown1E4**

**Unknown1E8** - flag

**Unknown1EC**

**Unknown220** - flag


## Example Structure
	<ParticleRuleDictionary>
		<Item>
			<Name>veh_exhaust_balloon_burner_flames</Name>
			<FxcFile>ptfx_sprite</FxcFile>
			<FxcTechnique>RGB_lit_soft</FxcTechnique>
			<Unknown10 value="2"/>
			<Unknown100 value="2"/>
			<Unknown104 value="1"/>
			<Unknown108 value="0"/>
			<Unknown10C value="0x10100"/>
			<Unknown118 value="10"/>
			<Unknown11C value="0"/>
			<Unknown1D0 value="2"/>
			<Unknown1E0 value="0"/>
			<Unknown1E4 value="0"/>
			<Unknown1E8 value="0x101"/>
			<Unknown1EC value="0"/>
			<Unknown220 value="0x2"/>
			<Spawner1>
      WIP
			</Spawner1>
			<Spawner2>
      WIP
			</Spawner2>
			<Behaviours>
      WIP
			</Behaviours>
			<ShaderVars>
      WIP
			</ShaderVars>
		</Item>
