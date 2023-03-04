# Particle Rule Properties
Particle Rules define properties and behaviour of individual particles, such as base speed, RGBA colors, light emission, shadow casting, shaders and textures used etc.  
[Example structure of a ParticleRule](#example-structure-of-the-entire-particlerule)

## Table of Contents
- [Header](#header)  
- [Spawners](#spawner1--spawner2)  
- [Behaviours](#behaviours)  
	- [Age](#age)
	- [Size](#size)
	- [Rotation](#rotation)
	- [Colour](#colour)
	- [AnimateTexture](#animatetexture)
	- [Velocity](#velocity)
	- [Acceleration](#acceleration)
	- [Wind](#wind)
	- [Dampening](#dampening)
	- [Collision](#collision)
	- [MatrixWeight](#matrixweight)
	- [Noise](#noise)
	- [Decal](#decal)
	- [FogVolume](#fogvolume)
	- [Sprite](#sprite)
	- [Trail](#trail)
	- [ZCull](#zcull)
- [ShaderVars](#shadervars)  
- [Example structure of a ParticleRule](#example-structure-of-the-entire-particlerule)

# Header
**Name** - Unique Particle Rule name, used to target it in EffectRuleDictionary  
**FxcFile** - .fxc shader dictionary name  
**FxcTechnique** - Shader technique name  

**Unknown10**  
**Unknown100**  
**Unknown104** - bool - Enables particle texture transparency  
**Unknown108**  
**Unknown10C** - flag  
**Unknown118** - _frames?_ - _Min texture animation speed?_  
**Unknown11C** - _frames?_ - _Max texture animation speed?_  
**Unknown1D0**  
**Unknown1E0**  
**Unknown1E4**  
**Unknown1E8** - flag  
**Unknown1EC**  
**Unknown220** - flag  

## 
# Spawner1 & Spawner2
_UNCONFIRMED_ - Attaches up to two different EffectRules to spawned particles?

**EffectRule** - Linked EffectRule name  
**Unknown18**  
**Unknown1C**  
**Unknown20**  
**Unknown24**  
**Unknown28**  
**Unknown38**  
**Unknown3C**  
**Unknown40**  
**Unknown44**  
**Unknown48**  
**Unknown68**  
**Unknown6C**  

## 
# Behaviours
All particle properties are described in this section.

### Example structure
	<Item>
		<Type value="Size"/>
		<Unknown270 value="0"/>
		<Unknown274 value="1"/>
		<KeyframeProperty0>
			<Name>ptxu_Size:m_whdMinKFP</Name>
			<Unknown6C value="256"/>
			<Keyframes/>
		</KeyframeProperty0>
		<KeyframeProperty1>
			<Name>ptxu_Size:m_whdMaxKFP</Name>
			<Unknown6C value="512"/>
			<Keyframes/>
		</KeyframeProperty1>
		<KeyframeProperty2>
			<Name>ptxu_Size:m_tblrScalarKFP</Name>
			<Unknown6C value="768"/>
			<Keyframes/>
		</KeyframeProperty2>
		<KeyframeProperty3>
			<Name>ptxu_Size:m_tblrVelScalarKFP</Name>
			<Unknown6C value="1024"/>
			<Keyframes/>
		</KeyframeProperty3>
	</Item>

### Unknown0 & Unknown4
These settings are universal for all keyframes in all KFP types.  
_UNCONFIRMED_ - define timeline position and lengh of each frame.  
Will be omitted in the following sections.

## Age
_Never used?_

## Size
**Unknown270** -  
**Unknown274** -  

### ptxu_Size:m_whdMinKFP
Minimal size of the particle  
_UNCONFIRMED_ - I have two ideas about these:  
1) Particle size is randomized between Min and Max (probable);
2) Particle goes from Min to Max through its lifetime (sensible).

Needs testing.  

**Unknown10** - Width  
**Unknown14** - Height  
**Unknown18** - Depth  
**Unknown1C** - 

### ptxu_Size:m_whdMaxKFP
Maximum size of the particle

**Unknown10** - Width  
**Unknown14** - Height  
**Unknown18** - Depth  
**Unknown1C** - 

### ptxu_Size:m_tblrScalarKFP
**Unknown10** -  
**Unknown14** -  
**Unknown18** -  
**Unknown1C** -  

### ptxu_Size:m_tblrVelScalarKFP
**Unknown10** -  
**Unknown14** -  
**Unknown18** -  
**Unknown1C** -  


## Rotation
**Unknown270** -  
**Unknown274** -  
**Unknown278** - _flag?_ -  
**Unknown27C** -  

### ptxu_Rotation:m_initialAngleMinKFP
**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  

### ptxu_Rotation:m_initialAngleMaxKFP
**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  

### ptxu_Rotation:m_angleMinKFP
Minimum target angle of the particle  

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  

### ptxu_Rotation:m_angleMaxKFP
Maximum target angle of the particle  

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  


## Colour
RGBA color tint applied to the particle and its emission brighteness. If particle texture has colors in it, the tint has to be count for them.  

**Unknown1E0** -  
**Unknown1E4** - _flag?_ -  

### ptxu_Colour:m_rgbaMinKFP
**Unknown10** - R  
**Unknown14** - G  
**Unknown18** - B  
**Unknown1C** - A  

### ptxu_Colour:m_rgbaMaxKFP
**Unknown10** - R  
**Unknown14** - G  
**Unknown18** - B  
**Unknown1C** - A  

### ptxu_Colour:m_emissiveIntensityKFP
**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** -  
**Unknown1C** -  


## AnimateTexture
**UnknownC0** -  
**UnknownC4** -  _Not tested. supp: framerate? target frame?_
**UnknownC8** -  
**UnknownCC** - _flag?_ -  

### ptxu_AnimateTexture:m_animRateKFP
**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** -  
**Unknown1C** -  


## Velocity

## Acceleration
**Unknown158** -  
**Unknown15C** -  

### ptxu_Acceleration:m_xyzMinKFP
**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  

### ptxu_Acceleration:m_xyzMaxKFP
**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** -  


## Wind
**UnknownD0** -  
**UnknownD4** -  
**UnknownD8** -  
**UnknownDC** -  
**UnknownE0** -  

### ptxu_Wind:m_influenceKFP
**Unknown10** - _Min?_  
**Unknown14** - _Max?_  
**Unknown18** -  
**Unknown1C** -  


## Dampening

## Collision

## MatrixWeight
**UnknownC0** - 

### ptxu_MatrixWeight:m_mtxWeightKFP
**Unknown10** -  
**Unknown14** -  
**Unknown18** -  
**Unknown1C** -  


## Noise

## Decal

## FogVolume

## Sprite
**Unknown30** -  
**Unknown34** -  
**Unknown38** -  
**Unknown40** -  
**Unknown44** -  
**Unknown48** -  
**Unknown4C** -  
**Unknown50** -  
**Unknown54** -  
**Unknown58** -  
**Unknown5C** - _flag?_ -  
**Unknown60** - _flag?_ -  


## Trail
**UnknownC4** -  
**UnknownC8** -  
**UnknownD4** -  
**UnknownD8** -  
**UnknownDC** -  
**UnknownE0** -  
**UnknownE4** -  
**UnknownEC** - _flag?_ -  

### ptxd_Trail:m_texInfoKFP
**Unknown10** -  
**Unknown14** -  
**Unknown18** -  
**Unknown1C** -  


## ZCull

##
# ShaderVars

### diffusetex2
Defines diffuse texture for the particle.  
Can use textures from other .ypt files if they're linked through **ptfxassetinfo.meta**.  

**Unknown18** -  
**Unknown3C** -  
**TextureName** - texture filename

	<Item>
		<Type value="Texture"/>
		<Name>diffusetex2</Name>
		<Unknown18 value="4"/>
		<Unknown3C value="1"/>
		<TextureName>_explosion_fireball</TextureName>
	</Item>
	
##
# Example structure of the entire ParticleRule
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
			<Unknown118 value="5"/>
			<Unknown11C value="0"/>
			<Unknown1D0 value="0"/>
			<Unknown1E0 value="0"/>
			<Unknown1E4 value="0"/>
			<Unknown1E8 value="0x101"/>
			<Unknown1EC value="0"/>
			<Unknown220 value="0x2"/>
			<Spawner1/>
			<Spawner2/>
			<Behaviours>
				<Item>
					<Type value="Size"/>
					<Unknown270 value="0"/>
					<Unknown274 value="1"/>
					<KeyframeProperty0>
						<Name>ptxu_Size:m_whdMinKFP</Name>
						<Unknown6C value="256"/>
						<Keyframes/>
					</KeyframeProperty0>
					<KeyframeProperty1>
						<Name>ptxu_Size:m_whdMaxKFP</Name>
						<Unknown6C value="512"/>
						<Keyframes/>
					</KeyframeProperty1>
					<KeyframeProperty2>
						<Name>ptxu_Size:m_tblrScalarKFP</Name>
						<Unknown6C value="768"/>
						<Keyframes/>
					</KeyframeProperty2>
					<KeyframeProperty3>
						<Name>ptxu_Size:m_tblrVelScalarKFP</Name>
						<Unknown6C value="1024"/>
						<Keyframes/>
					</KeyframeProperty3>
				</Item>
			<ShaderVars>
				<Item>
						<Type value="Texture"/>
						<Name>diffusetex2</Name>
						<Unknown18 value="4"/>
						<Unknown3C value="1"/>
						<TextureName>_explosion_fireball</TextureName>
				</Item>
			</ShaderVars>
		</Item>
