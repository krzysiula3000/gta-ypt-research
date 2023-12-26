# Keyframe properties research
Contributors: @krzysiula, @w_33_by

##
`DISCLAIMER` keep in mind many things i say here may be partially or completely incorrect, if i'm not 100% sure about an information                               
i will put "`OPINION`" next to it, if i'm wrong just contact me i will change anything that's incorrect
               


From what i understand after playing with the file, many particle effects don't have a dedicated mesh, only a plane that's automatically                            
generated and the texture specified in the .ypt is applied onto it, whenever the particle plays
 
 
Many keyframe properties have 2 variations, one with `Min` and the other with `Max` in their names, when the two values are not exactly equal, the game will use a random value from within that range


### Unknown6C - every next UNK6C is 256 bigger than the previous one, starting value = 256, `OPINION`, it functions as an index of some sort
_when adding more keyframe properties it's not necessary to keep the order of unk6c, you can use any value and it will work just fine,
		it probably works like YMAP's GUID)_
## **EffectRuleDictionary's keyframe properties:** 

### ptxEmitterRule:m_playbackRateScalarKFP ## where KFP stands for keyframe property

- [scales all keyframes](https://imgur.com/a/FvOQz9k)

            <Unknown0 value="0"/>
            <Unknown4 value="0"/>
            <Unknown10 value="1"/>   Playback rate factor
            <Unknown14 value="0.01"/>   Always 0.01
            <Unknown18 value="0.01"/>   Always 0.01
            <Unknown1C value="0.01"/>   Always 0.01

### ptxEffectRule:m_dataSphereKFP
-  unknown

### ptxEffectRule:m_zoomScalarKFP

- responsible for scaling [emitters](https://imgur.com/a/VsYK1X0)

       	    <Unknown0 value="0" />
       	    <Unknown4 value="0" />
       	    <Unknown10 value="700" />   X axis
       	    <Unknown14 value="800" />  Y axis
       	    <Unknown18 value="0" />   Z axis
       	    <Unknown1C value="0" />
	   
     
### ptxEmitterRule:m_sizeScalarKFP
- responsible for scaling [emitters](https://imgur.com/a/VsYK1X0)

            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="254.5414" />   X axis
            <Unknown14 value="254.5414" />   Y axis
            <Unknown18 value="254.5414" />   Z axis
            <Unknown1C value="100" /> ?
            
### ptxEmitterRule:m_spawnRateOverTimeKFP
- reponsible for spawning [emitters](https://imgur.com/a/VsYK1X0) over time (probably measured in frames) 
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="10" /> ?
            <Unknown14 value="10" /> ?
            <Unknown18 value="10" /> ?
            <Unknown1C value="0" /> ?

### ptxu_Colour:m_rgbaMinKFP 
- changes the color of the texture
 
            <Unknown0 value="0" />   ?
            <Unknown4 value="0" />   ?
            <Unknown10 value="0.705179" />   red channel (values 0-1)
            <Unknown14 value="0.732523" />   green channel (values 0-1)
            <Unknown18 value="0.705179" />   blue channel (values 0-1)
            <Unknown1C value="1" />   alpha channel (values 0-1)
            
### ptxEmitterRule:m_particleLifeKFP
- changes the lifespan of the [particle](https://imgur.com/a/VsYK1X0)
 
            <Unknown0 value="0" />   always set to 0
            <Unknown4 value="0" />   always set to 0
            <Unknown10 value="2" />   value changing the particle life's lenght
            <Unknown14 value="3" />   value changing the particle life's lenght
            <Unknown18 value="0.01" />   typically set to 0 or 0.01
            <Unknown1C value="0.01" />   typically set to 0 or 0.01

### ptxEmitterRule:m_spawnRateOverTimeKFP
- affects the spawn rate over time
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="5" />   value affecting it
            <Unknown14 value="9" />   value affecting it
            <Unknown18 value="0" /> ?
            <Unknown1C value="0" /> ?

===========================================================================

## **EmitterRuleDictionary's keyframe properties:**  




### ptxCreationDomain:m_positionKFP
- specifies [emitter's](https://imgur.com/a/VsYK1X0) offset upon spawning
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="-0.02" />   X axis
            <Unknown14 value="0.04" />   Y axis
            <Unknown18 value="-0.02" />   Z axis
            <Unknown1C value="0" /> ?

### ptxTargetDomain:m_positionKFP
- specifies the position the [emitter](https://imgur.com/a/VsYK1X0) is gonna end up at
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="0.014" />   X axis
            <Unknown14 value="-2" />   Y axis
            <Unknown18 value="0" />   Z axis
            <Unknown1C value="0" /> ?
            
### ptxCreationDomain:m_rotationKFP
- specifies [emitter's](https://imgur.com/a/VsYK1X0) rotation upon spawning
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="90" />   X axis, measured in degrees
            <Unknown14 value="0" />   Y axis, measured in degrees
            <Unknown18 value="0" />   Z axis, measured in degrees
            <Unknown1C value="0" /> ?
            
### ptxTargetDomain:m_sizeOuterKFP
- ptxTargetDomain:m_sizeOuterKFP and ptxTargetDomain:m_sizeInnerKFP define the target domain area size, i.e. the area which the [particles](https://imgur.com/a/VsYK1X0) will move towards as they live. The inner sphere can be enlarged to force [particles](https://imgur.com/a/VsYK1X0) away from the centre of the domain area, outer sphere limits their spread. Same for the creation domain https://imgur.com/a/iigppl6
 
            
### ptxEmitterRule:m_spawnRateOverDistKFP
- spawn rate over distance
 
            
### ptxEmitterRule:m_speedScalarKFP
- `OPINION` scales speed of the [emitter](https://imgur.com/a/VsYK1X0) (probably multiplies the speed given by some other KFP)
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="254.5414" />   X axis
            <Unknown14 value="254.5414" />   Y axis
            <Unknown18 value="254.5414" />   Z axis
            <Unknown1C value="100" /> ?
            
### ptxEmitterRule:m_accnScalarKFP
- affects [emitter's](https://imgur.com/a/VsYK1X0) acceleration, values can be negative
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="0.8" />   x axis
            <Unknown14 value="1.4" />   y axis
            <Unknown18 value="0" />   z axis
            <Unknown1C value="0" /> ?
            
### ptxEmitterRule:m_matrixWeightScalarKFP
- unknown


### ptxEmitterRule:m_dampeningScalarKFP
- `OPINION` It seems to dampen the movement of [particles](https://imgur.com/a/VsYK1X0) in specified directions, adds some inertia to them
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ? 
            <Unknown10 value="100" />   x axis?
            <Unknown14 value="100" />   y axis?
            <Unknown18 value="0" />   z axis?
            <Unknown1C value="0" /> ?
            
### ptxEmitterRule:m_inheritVelocityKFP
- specifies the [emitter's](https://imgur.com/a/VsYK1X0) velocity 
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ? 
            <Unknown10 value="100" />   x axis
            <Unknown14 value="100" />   y axis
            <Unknown18 value="0" />   z axis
            <Unknown1C value="0" /> ?
        
        
===========================================================================
 
## **ParticleRuleDictionary's keyframe properties:** 

            
### ptxu_Acceleration:m_xyzMinKFP
- specifies the acceleration of [particle](https://imgur.com/a/VsYK1X0), values can be negative
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="1.5" />   x axis
            <Unknown14 value="-2.2" />   y axis
            <Unknown18 value="1.2" />   z axis
            <Unknown1C value="0" /> ?
            
### ptxu_Rotation:m_initialAngleMinKFP
- specifies the [particle's](https://imgur.com/a/VsYK1X0) angle upon spawning
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="-35" />   x axis, measured in degrees
            <Unknown14 value="0" />   y axis, measured in degrees
            <Unknown18 value="0" />   z axis, measured in degrees
            <Unknown1C value="0" /> ?
            
### ptxu_Rotation:m_angleMinKFP 
- specifies the rotation the [particle](https://imgur.com/a/VsYK1X0) will target
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="10" />   x axis, measured in degrees
            <Unknown14 value="0" />   y axis, measured in degrees
            <Unknown18 value="0" />   z axis, measured in degrees
            <Unknown1C value="0" /> ?
            
### ptxu_Size:m_whdMinKFP 
- specifies the size of [particle](https://imgur.com/a/VsYK1X0), whd stands for width, height, depth
 
            <Unknown0 value="0" />   
            <Unknown4 value="0" />   
            <Unknown10 value="0.2" />   x axis
            <Unknown14 value="0.2" />   y axis
            <Unknown18 value="0" />   z axis
            <Unknown1C value="0" />   
            
### ptxu_AnimateTexture:m_animRateKFP
- uv animation using sprite sheet
 
            
### ptxu_Size:m_tblrScalarKFP
- related to size
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="1" />   x axis??
            <Unknown14 value="1" />   y axis??
            <Unknown18 value="1" />   z axis??
            <Unknown1C value="1" /> ?
            
### Wind
- not a keyframe property, specifies wind direction and speed, affects emitters with ptxu_Wind:m_influenceKFP
 
     	      <Type value="Wind" />
     	      <UnknownD0 value="20" />
     	      <UnknownD4 value="50" />
     	      <UnknownD8 value="1" />
     	      <UnknownDC value="2" />
     	      <UnknownE0 value="0" />
            
### ptxu_Wind:m_influenceKFP
- specifies how much will the [particle](https://imgur.com/a/VsYK1X0) be affected by wind 
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="0" />   x axis??
            <Unknown14 value="0" />   y axis??
            <Unknown18 value="0" />   z axis??
            <Unknown1C value="0" /> ?
            
### ptxu_Noise:m_velNoiseMineKFP
- introduces noise to [particle's](https://imgur.com/a/VsYK1X0) velocity
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="1" />   x axis
            <Unknown14 value="1" />   y axis
            <Unknown18 value="0" />   z axis
            <Unknown1C value="0" /> ?
            
            
### ptxu_Noise:m_posNoiseMinKFP
- introduces noise to [particle's](https://imgur.com/a/VsYK1X0) position
 
            <Unknown0 value="0" /> ?
            <Unknown4 value="0" /> ?
            <Unknown10 value="1" />   x axis
            <Unknown14 value="1" />   y axis
            <Unknown18 value="0" />   z axis
            <Unknown1C value="0" /> ?
            
