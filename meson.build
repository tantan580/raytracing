project(
    'raytracing',
    'c',
	'cpp',
    version: '0.1.0',
    license: 'MIT',
    meson_version: '>=0.53.0',
	default_options: [
		'cpp_std=c++17',
		'c_std=c11',
		'warning_level=3',
		'werror=false',
	],
)

demo_srcs = {
    'main_00' : {
        'src' : 'main_00.cc',
    },
}

foreach name, info : demo_srcs
    executable(
        name, 
        info.get('src'),
        dependencies: info.get('deps', []),
        include_directories : include_directories('.'),
    )
endforeach