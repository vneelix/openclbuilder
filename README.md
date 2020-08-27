# openclbuilder
Simple OpenCL program builder for C.
CL Builder use support structure
```C
typedef struct	s_cl_builder {
	cl_platform_id		platform;
	cl_device_id		device;
	cl_context		context;
	cl_command_queue	queue;
	cl_program		program;
}				t_cl_builder;
```
Signature is ```C openclbuilder(t_cl_builder *cl, char *src_dir, char *inc_dir)```
